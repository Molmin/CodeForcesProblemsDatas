## Description

<div><p>Gerald is very particular to eight point sets. He thinks that any decent eight point set must consist of all pairwise intersections of three distinct integer vertical straight lines and three distinct integer horizontal straight lines, except for the average of these nine points. In other words, there must be three integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">3</sub></span> and three more integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">3</sub></span>, such that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; <i>x</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> &lt; <i>y</i><sub class="lower-index">3</sub></span> and the eight point set consists of all points <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub>)</span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ 3</span>), except for point <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>.</p><p>You have a set of eight points. Find out if Gerald can use this set?</p></div><div class="input-specification"><p>The input consists of eight lines, the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). You do not have any other conditions for these points.</p></div><div class="output-specification"><p>In a single line print word "<span class="tex-font-style-tt">respectable</span>", if the given set of points corresponds to Gerald's decency rules, and "<span class="tex-font-style-tt">ugly</span>" otherwise.</p></div>

## Input

<p>The input consists of eight lines, the <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). You do not have any other conditions for these points.</p>

## Output

<p>In a single line print word "<span class="tex-font-style-tt">respectable</span>", if the given set of points corresponds to Gerald's decency rules, and "<span class="tex-font-style-tt">ugly</span>" otherwise.</p>





```input1
0 0
0 1
0 2
1 0
1 2
2 0
2 1
2 2

```




```input2
0 0
1 0
2 0
3 0
4 0
5 0
6 0
7 0

```




```input3
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2

```




```output1
respectable

```




```output2
ugly

```




```output3
ugly

```


