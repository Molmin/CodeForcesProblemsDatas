## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> distinct points on a plane with integral coordinates. For each point you can either draw a vertical line through it, draw a horizontal line through it, or do nothing.</p><p>You consider several coinciding straight lines as a single one. How many distinct pictures you can get? Print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of points.</p><p><span class="tex-span"><i>n</i></span> lines follow. The (<span class="tex-span"><i>i</i> + 1</span>)-th of these lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th point.</p><p>It is guaranteed that all points are distinct.</p></div><div class="output-specification"><p>Print the number of possible distinct pictures modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of points.</p><p><span class="tex-span"><i>n</i></span> lines follow. The (<span class="tex-span"><i>i</i> + 1</span>)-th of these lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the <span class="tex-span"><i>i</i></span>-th point.</p><p>It is guaranteed that all points are distinct.</p>

## Output

<p>Print the number of possible distinct pictures modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4
1 1
1 2
2 1
2 2

```




```input2
2
-1 -1
0 1

```




```output1
16

```




```output2
9

```



## Note

<p>In the first example there are two vertical and two horizontal lines passing through the points. You can get pictures with any subset of these lines. For example, you can get the picture containing all four lines in two ways (each segment represents a line containing it).</p><center> The first way:   <img class="tex-graphics" height="151px" src="file://na3wIeao.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px">   The second way:   <img class="tex-graphics" height="151px" src="file://bppL17eZ.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px">   </center><p>In the second example you can work with two points independently. The number of pictures is <span class="tex-span">3<sup class="upper-index">2</sup> = 9</span>.</p>
