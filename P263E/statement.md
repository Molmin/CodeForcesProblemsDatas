## Description

<div><p>You've got a table of size <span class="tex-span"><i>n</i> × <i>m</i></span>. On the intersection of the <span class="tex-span"><i>i</i></span>-th row (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) and the <span class="tex-span"><i>j</i></span>-th column (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) there is a non-negative integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. Besides, you've got a non-negative integer <span class="tex-span"><i>k</i></span>.</p><p>Your task is to find such pair of integers <span class="tex-span">(<i>a</i>, <i>b</i>)</span> that meets these conditions: </p><ul> <li> <span class="tex-span"><i>k</i> ≤ <i>a</i> ≤ <i>n</i> - <i>k</i> + 1</span>; </li><li> <span class="tex-span"><i>k</i> ≤ <i>b</i> ≤ <i>m</i> - <i>k</i> + 1</span>; </li><li> let's denote the maximum of the function <img align="middle" class="tex-formula" src="file://wIqInwLP.png" style="max-width: 100.0%;max-height: 100.0%;"> among all integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, that satisfy the inequalities <span class="tex-span"><i>k</i> ≤ <i>x</i> ≤ <i>n</i> - <i>k</i> + 1</span> and <span class="tex-span"><i>k</i> ≤ <i>y</i> ≤ <i>m</i> - <i>k</i> + 1</span>, as <span class="tex-span"><i>mval</i></span>; for the required pair of numbers the following equation must hold <span class="tex-span"><i>f</i>(<i>a</i>, <i>b</i>) = <i>mval</i></span>. </li></ul></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <img align="middle" class="tex-formula" src="file://O0vcN7Tz.png" style="max-width: 100.0%;max-height: 100.0%;">). Next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>m</i></span> integers: the <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line equals <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The numbers in the lines are separated by spaces.</p></div><div class="output-specification"><p>Print the required pair of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Separate the numbers by a space.</p><p>If there are multiple correct answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>, <img align="middle" class="tex-formula" src="file://O0vcN7Tz.png" style="max-width: 100.0%;max-height: 100.0%;">). Next <span class="tex-span"><i>n</i></span> lines each contains <span class="tex-span"><i>m</i></span> integers: the <span class="tex-span"><i>j</i></span>-th number on the <span class="tex-span"><i>i</i></span>-th line equals <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The numbers in the lines are separated by spaces.</p>

## Output

<p>Print the required pair of integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Separate the numbers by a space.</p><p>If there are multiple correct answers, you are allowed to print any of them.</p>





```input1
4 4 2
1 2 3 4
1 1 1 1
2 2 2 2
4 3 2 1

```




```input2
5 7 3
8 2 3 4 2 3 3
3 4 6 2 3 4 6
8 7 6 8 4 5 7
1 2 3 2 1 3 2
4 5 3 2 1 2 1

```




```output1
3 2

```




```output2
3 3

```


