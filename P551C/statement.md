## Description

<div><p>Professor GukiZ is concerned about making his way to school, because massive piles of boxes are blocking his way. </p><p>In total there are <span class="tex-span"><i>n</i></span> piles of boxes, arranged in a line, from left to right, <span class="tex-span"><i>i</i></span>-th pile (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) containing <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> boxes. Luckily, <span class="tex-span"><i>m</i></span> students are willing to help GukiZ by removing all the boxes from his way. Students are working simultaneously. At time <span class="tex-span">0</span>, all students are located left of the first pile. It takes one second for every student to move from this position to the first pile, and after that, every student must start performing sequence of two possible operations, each taking one second to complete. Possible operations are:</p><ol><li> If <span class="tex-span"><i>i</i> ≠ <i>n</i></span>, move from pile <span class="tex-span"><i>i</i></span> to pile <span class="tex-span"><i>i</i> + 1</span>;</li><li> If pile located at the position of student is not empty, remove one box from it.</li></ol><p>GukiZ's students aren't smart at all, so they need you to tell them how to remove boxes before professor comes (he is very impatient man, and doesn't want to wait). They ask you to calculate minumum time <span class="tex-span"><i>t</i></span> in seconds for which they can remove all the boxes from GukiZ's way. Note that students can be positioned in any manner after <span class="tex-span"><i>t</i></span> seconds, but all the boxes must be removed.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of piles of boxes and the number of GukiZ's students. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the number of boxes on <span class="tex-span"><i>i</i></span>-th pile. It's guaranteed that at least one pile of is non-empty.</p></div><div class="output-specification"><p>In a single line, print one number, minimum time needed to remove all the boxes in seconds.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of piles of boxes and the number of GukiZ's students. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the number of boxes on <span class="tex-span"><i>i</i></span>-th pile. It's guaranteed that at least one pile of is non-empty.</p>

## Output

<p>In a single line, print one number, minimum time needed to remove all the boxes in seconds.</p>





```input1
2 1
1 1

```




```input2
3 2
1 0 2

```




```input3
4 100
3 4 5 4

```




```output1
4

```




```output2
5

```




```output3
5

```



## Note

<p>First sample: Student will first move to the first pile (<span class="tex-span">1</span> second), then remove box from first pile (<span class="tex-span">1</span> second), then move to the second pile (<span class="tex-span">1</span> second) and finally remove the box from second pile (<span class="tex-span">1</span> second).</p><p>Second sample: One of optimal solutions is to send one student to remove a box from the first pile and a box from the third pile, and send another student to remove a box from the third pile. Overall, <span class="tex-span">5</span> seconds.</p><p>Third sample: With a lot of available students, send three of them to remove boxes from the first pile, four of them to remove boxes from the second pile, five of them to remove boxes from the third pile, and four of them to remove boxes from the fourth pile. Process will be over in <span class="tex-span">5</span> seconds, when removing the boxes from the last pile is finished.</p>
