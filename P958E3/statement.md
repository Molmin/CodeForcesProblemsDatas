## Description

<div><p>Now that Heidi knows that she can assign Rebel spaceships to bases (recall the easy subtask), she is asking you: how <span class="tex-font-style-it">exactly</span> to do this? Now, given positions of <span class="tex-span"><i>N</i></span> spaceships and <span class="tex-span"><i>N</i></span> bases on a plane, your task is to connect spaceships and bases with line segments so that: </p><ul> <li> The segments do not intersect. </li><li> Such a connection forms a perfect matching. </li></ul></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). For <span class="tex-span">1 ≤ <i>i</i> ≤ <i>N</i></span>, the <span class="tex-span"><i>i</i> + 1</span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10000</span>) denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th spaceship. The following <span class="tex-span"><i>N</i></span> lines have the same format, denoting the position of bases. It is guaranteed that no two points coincide and no three points are on the same line.</p></div><div class="output-specification"><p>The output should have <span class="tex-span"><i>N</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain an integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, the index of the base to which the <span class="tex-span"><i>i</i></span>-th spaceship is connected. The sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>N</i></sub></span> should form a permutation of <span class="tex-span">1, ..., <i>N</i></span>.</p><p>It is guaranteed that a solution exists. If there are multiple solutions, you can output any one of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>). For <span class="tex-span">1 ≤ <i>i</i> ≤ <i>N</i></span>, the <span class="tex-span"><i>i</i> + 1</span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10000</span>) denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th spaceship. The following <span class="tex-span"><i>N</i></span> lines have the same format, denoting the position of bases. It is guaranteed that no two points coincide and no three points are on the same line.</p>

## Output

<p>The output should have <span class="tex-span"><i>N</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain an integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, the index of the base to which the <span class="tex-span"><i>i</i></span>-th spaceship is connected. The sequence <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>N</i></sub></span> should form a permutation of <span class="tex-span">1, ..., <i>N</i></span>.</p><p>It is guaranteed that a solution exists. If there are multiple solutions, you can output any one of them.</p>





```input1
4
6 6
5 1
2 4
4 0
5 4
1 2
2 1
3 5

```




```output1
4
1
2
3

```


