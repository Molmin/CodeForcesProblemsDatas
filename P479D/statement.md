## Description

<div><p>Valery is a PE teacher at a school in Berland. Soon the students are going to take a test in long jumps, and Valery has lost his favorite ruler! </p><p>However, there is no reason for disappointment, as Valery has found another ruler, its length is <span class="tex-span"><i>l</i></span> centimeters. The ruler already has <span class="tex-span"><i>n</i></span> marks, with which he can make measurements. We assume that the marks are numbered from 1 to <span class="tex-span"><i>n</i></span> in the order they appear from the beginning of the ruler to its end. The first point coincides with the beginning of the ruler and represents the origin. The last mark coincides with the end of the ruler, at distance <span class="tex-span"><i>l</i></span> from the origin. This ruler can be repesented by an increasing sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the distance of the <span class="tex-span"><i>i</i></span>-th mark from the origin (<span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> = <i>l</i></span>).</p><p>Valery believes that with a ruler he can measure the distance of <span class="tex-span"><i>d</i></span> centimeters, if there is a pair of integers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i></span>), such that the distance between the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th mark is exactly equal to <span class="tex-span"><i>d</i></span> (in other words, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> - <i>a</i><sub class="lower-index"><i>i</i></sub> = <i>d</i></span>). </p><p>Under the rules, the girls should be able to jump at least <span class="tex-span"><i>x</i></span> centimeters, and the boys should be able to jump at least <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>x</i> &lt; <i>y</i></span>) centimeters. To test the children's abilities, Valery needs a ruler to measure each of the distances <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. </p><p>Your task is to determine what is the minimum number of additional marks you need to add on the ruler so that they can be used to measure the distances <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. Valery can add the marks at any integer non-negative distance from the origin not exceeding the length of the ruler.</p></div><div class="input-specification"><p>The first line contains four positive space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>l</i></span>) — the number of marks, the length of the ruler and the jump norms for girls and boys, correspondingly.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 = <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> = <i>l</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> shows the distance from the <span class="tex-span"><i>i</i></span>-th mark to the origin.</p></div><div class="output-specification"><p>In the first line print a single non-negative integer <span class="tex-span"><i>v</i></span> — the minimum number of marks that you need to add on the ruler.</p><p>In the second line print <span class="tex-span"><i>v</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>v</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>l</i></span>). Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th mark should be at the distance of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> centimeters from the origin. Print the marks in any order. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains four positive space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>l</i></span>) — the number of marks, the length of the ruler and the jump norms for girls and boys, correspondingly.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 = <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> = <i>l</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> shows the distance from the <span class="tex-span"><i>i</i></span>-th mark to the origin.</p>

## Output

<p>In the first line print a single non-negative integer <span class="tex-span"><i>v</i></span> — the minimum number of marks that you need to add on the ruler.</p><p>In the second line print <span class="tex-span"><i>v</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>v</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>l</i></span>). Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that the <span class="tex-span"><i>i</i></span>-th mark should be at the distance of <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> centimeters from the origin. Print the marks in any order. If there are multiple solutions, print any of them.</p>





```input1
3 250 185 230
0 185 250

```




```input2
4 250 185 230
0 20 185 250

```




```input3
2 300 185 230
0 300

```




```output1
1
230

```




```output2
0

```




```output3
2
185 230

```



## Note

<p>In the first sample it is impossible to initially measure the distance of <span class="tex-span">230</span> centimeters. For that it is enough to add a <span class="tex-span">20</span> centimeter mark or a <span class="tex-span">230</span> centimeter mark.</p><p>In the second sample you already can use the ruler to measure the distances of <span class="tex-span">185</span> and <span class="tex-span">230</span> centimeters, so you don't have to add new marks.</p><p>In the third sample the ruler only contains the initial and the final marks. We will need to add two marks to be able to test the children's skills.</p>
