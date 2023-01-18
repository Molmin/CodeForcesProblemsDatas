## Description

<div><p>Bob has a rectangular chocolate bar of the size <span class="tex-span"><i>W</i> × <i>H</i></span>. He introduced a cartesian coordinate system so that the point <span class="tex-span">(0, 0)</span> corresponds to the lower-left corner of the bar, and the point <span class="tex-span">(<i>W</i>, <i>H</i>)</span> corresponds to the upper-right corner. Bob decided to split the bar into pieces by breaking it. Each break is a segment parallel to one of the coordinate axes, which connects the edges of the bar. More formally, each break goes along the line <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index"><i>c</i></sub></span> or <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index"><i>c</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>c</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>c</i></sub></span> are integers. It should divide one part of the bar into two non-empty parts. After Bob breaks some part into two parts, he breaks the resulting parts <span class="tex-font-style-bf">separately and independently from each other</span>. Also he doesn't move the parts of the bar. Bob made <span class="tex-span"><i>n</i></span> breaks and wrote them down in his notebook in arbitrary order. At the end he got <span class="tex-span"><i>n</i> + 1</span> parts. Now he wants to calculate their areas. Bob is lazy, so he asks you to do this task.</p></div><div class="input-specification"><p>The first line contains 3 integers <span class="tex-span"><i>W</i></span>, <span class="tex-span"><i>H</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>W</i>, <i>H</i>, <i>n</i> ≤ 100</span>) — width of the bar, height of the bar and amount of breaks. Each of the following <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 2</sub></span> — coordinates of the endpoints of the <span class="tex-span"><i>i</i></span>-th break (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i>, 1</sub> ≤ <i>x</i><sub class="lower-index"><i>i</i>, 2</sub> ≤ <i>W</i>, 0 ≤ <i>y</i><sub class="lower-index"><i>i</i>, 1</sub> ≤ <i>y</i><sub class="lower-index"><i>i</i>, 2</sub> ≤ <i>H</i></span>, or <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub> = <i>x</i><sub class="lower-index"><i>i</i>, 2</sub></span>, or <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i>, 1</sub> = <i>y</i><sub class="lower-index"><i>i</i>, 2</sub></span>). Breaks are given in arbitrary order.</p><p>It is guaranteed that the set of breaks is correct, i.e. there is some order of the given breaks that each next break divides exactly one part of the bar into two non-empty parts.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i> + 1</span> numbers — areas of the resulting parts in the increasing order.</p></div>

## Input

<p>The first line contains 3 integers <span class="tex-span"><i>W</i></span>, <span class="tex-span"><i>H</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>W</i>, <i>H</i>, <i>n</i> ≤ 100</span>) — width of the bar, height of the bar and amount of breaks. Each of the following <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 2</sub></span> — coordinates of the endpoints of the <span class="tex-span"><i>i</i></span>-th break (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i>, 1</sub> ≤ <i>x</i><sub class="lower-index"><i>i</i>, 2</sub> ≤ <i>W</i>, 0 ≤ <i>y</i><sub class="lower-index"><i>i</i>, 1</sub> ≤ <i>y</i><sub class="lower-index"><i>i</i>, 2</sub> ≤ <i>H</i></span>, or <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub> = <i>x</i><sub class="lower-index"><i>i</i>, 2</sub></span>, or <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i>, 1</sub> = <i>y</i><sub class="lower-index"><i>i</i>, 2</sub></span>). Breaks are given in arbitrary order.</p><p>It is guaranteed that the set of breaks is correct, i.e. there is some order of the given breaks that each next break divides exactly one part of the bar into two non-empty parts.</p>

## Output

<p>Output <span class="tex-span"><i>n</i> + 1</span> numbers — areas of the resulting parts in the increasing order.</p>





```input1
2 2 2
1 0 1 2
0 1 1 1

```




```input2
2 2 3
1 0 1 2
0 1 1 1
1 1 2 1

```




```input3
2 4 2
0 1 2 1
0 3 2 3

```




```output1
1 1 2
```




```output2
1 1 1 1
```




```output3
2 2 4
```


