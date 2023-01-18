## Description

<div><p>Vasya is interested in arranging dominoes. He is fed up with common dominoes and he uses the dominoes of different heights. He put <span class="tex-span"><i>n</i></span> dominoes on the table along one axis, going from left to right. Every domino stands perpendicular to that axis so that the axis passes through the center of its base. The <span class="tex-span"><i>i</i></span>-th domino has the coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and the height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Now Vasya wants to learn for every domino, how many dominoes will fall if he pushes it to the right. Help him do that. </p><p>Consider that a domino falls if it is touched strictly above the base. In other words, the fall of the domino with the initial coordinate <span class="tex-span"><i>x</i></span> and height <span class="tex-span"><i>h</i></span> leads to the fall of all dominoes on the segment <span class="tex-span">[<i>x</i> + 1, <i>x</i> + <i>h</i> - 1]</span>.</p><center><img class="tex-graphics" src="file://AswPWS5K.png" style="max-width: 100.0%;max-height: 100.0%;"></center></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which is the number of dominoes. Then follow <span class="tex-span"><i>n</i></span> lines containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>, 2 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) each, which are the coordinate and height of every domino. No two dominoes stand on one point.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> — the number of dominoes that will fall if Vasya pushes the <span class="tex-span"><i>i</i></span>-th domino to the right (including the domino itself).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which is the number of dominoes. Then follow <span class="tex-span"><i>n</i></span> lines containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>, 2 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) each, which are the coordinate and height of every domino. No two dominoes stand on one point.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> — the number of dominoes that will fall if Vasya pushes the <span class="tex-span"><i>i</i></span>-th domino to the right (including the domino itself).</p>





```input1
4
16 5
20 5
10 10
18 2

```




```input2
4
0 10
1 5
9 10
15 10

```




```output1
3 1 4 1
```




```output2
4 1 2 1
```


