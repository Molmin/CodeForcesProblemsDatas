## Description

<div><p>Pashmak has fallen in love with an attractive girl called Parmida since one year ago...</p><p>Today, Pashmak set up a meeting with his partner in a romantic garden. Unfortunately, Pashmak has forgotten where the garden is. But he remembers that the garden looks like a square with sides parallel to the coordinate axes. He also remembers that there is exactly one tree on each vertex of the square. Now, Pashmak knows the position of only two of the trees. Help him to find the position of two remaining ones.</p></div><div class="input-specification"><p>The first line contains four space-separated <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span">( - 100 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 100)</span> integers, where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> are coordinates of the first tree and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are coordinates of the second tree. It's guaranteed that the given points are distinct.</p></div><div class="output-specification"><p>If there is no solution to the problem, print <span class="tex-font-style-tt">-1</span>. Otherwise print four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>, <i>y</i><sub class="lower-index">4</sub></span> that correspond to the coordinates of the two other trees. If there are several solutions you can output any of them. </p><p>Note that <span class="tex-span"><i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>, <i>y</i><sub class="lower-index">4</sub></span> must be in the range <span class="tex-span">( - 1000 ≤ <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>, <i>y</i><sub class="lower-index">4</sub> ≤ 1000)</span>.</p></div>

## Input

<p>The first line contains four space-separated <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span">( - 100 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 100)</span> integers, where <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> are coordinates of the first tree and <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> are coordinates of the second tree. It's guaranteed that the given points are distinct.</p>

## Output

<p>If there is no solution to the problem, print <span class="tex-font-style-tt">-1</span>. Otherwise print four space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>, <i>y</i><sub class="lower-index">4</sub></span> that correspond to the coordinates of the two other trees. If there are several solutions you can output any of them. </p><p>Note that <span class="tex-span"><i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>, <i>y</i><sub class="lower-index">4</sub></span> must be in the range <span class="tex-span">( - 1000 ≤ <i>x</i><sub class="lower-index">3</sub>, <i>y</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>, <i>y</i><sub class="lower-index">4</sub> ≤ 1000)</span>.</p>





```input1
0 0 0 1

```




```input2
0 0 1 1

```




```input3
0 0 1 2

```




```output1
1 0 1 1

```




```output2
0 1 1 0

```




```output3
-1

```


