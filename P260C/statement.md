## Description

<div><p>Little Vasya had <span class="tex-span"><i>n</i></span> boxes with balls in the room. The boxes stood in a row and were numbered with numbers from 1 to <span class="tex-span"><i>n</i></span> from left to right.</p><p>Once Vasya chose one of the boxes, let's assume that its number is <span class="tex-span"><i>i</i></span>, took all balls out from it (it is guaranteed that this box originally had at least one ball), and began putting balls (one at a time) to the boxes with numbers <span class="tex-span"><i>i</i> + 1</span>, <span class="tex-span"><i>i</i> + 2</span>, <span class="tex-span"><i>i</i> + 3</span> and so on. If Vasya puts a ball into the box number <span class="tex-span"><i>n</i></span>, then the next ball goes to box <span class="tex-span">1</span>, the next one goes to box <span class="tex-span">2</span> and so on. He did it until he had no balls left in his hands. It is possible that Vasya puts multiple balls to the same box, and it is also possible that one or more balls will go to the box number <span class="tex-span"><i>i</i></span>. If <span class="tex-span"><i>i</i> = <i>n</i></span>, Vasya puts the first ball into the box number <span class="tex-span">1</span>, then the next ball goes to box <span class="tex-span">2</span> and so on. </p><p>For example, let's suppose that initially Vasya had four boxes, and the first box had <span class="tex-span">3</span> balls, the second one had <span class="tex-span">2</span>, the third one had <span class="tex-span">5</span> and the fourth one had <span class="tex-span">4</span> balls. Then, if <span class="tex-span"><i>i</i> = 3</span>, then Vasya will take all five balls out of the third box and put them in the boxes with numbers: <span class="tex-span">4, 1, 2, 3, 4</span>. After all Vasya's actions the balls will lie in the boxes as follows: in the first box there are <span class="tex-span">4</span> balls, <span class="tex-span">3</span> in the second one, <span class="tex-span">1</span> in the third one and <span class="tex-span">6</span> in the fourth one.</p><p>At this point Vasya has completely forgotten the original arrangement of the balls in the boxes, but he knows how they are arranged now, and the number <span class="tex-span"><i>x</i></span> — the number of the box, where he put the last of the taken out balls.</p><p>He asks you to help to find the initial arrangement of the balls in the boxes.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), that represent the number of the boxes and the index of the box that got the last ball from Vasya, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub> ≠ 0</span>) represents the number of balls in the box with index <span class="tex-span"><i>i</i></span> after Vasya completes all the actions. </p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th one represents the number of balls in the box number <span class="tex-span"><i>i</i></span> before Vasya starts acting. Separate the numbers in the output by spaces. If there are multiple correct solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), that represent the number of the boxes and the index of the box that got the last ball from Vasya, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub> ≠ 0</span>) represents the number of balls in the box with index <span class="tex-span"><i>i</i></span> after Vasya completes all the actions. </p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th one represents the number of balls in the box number <span class="tex-span"><i>i</i></span> before Vasya starts acting. Separate the numbers in the output by spaces. If there are multiple correct solutions, you are allowed to print any of them.</p>





```input1
4 4
4 3 1 6

```




```input2
5 2
3 2 0 2 7

```




```input3
3 3
2 3 1

```




```output1
3 2 5 4
```




```output2
2 1 4 1 6
```




```output3
1 2 3
```


