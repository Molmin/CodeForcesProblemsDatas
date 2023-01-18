## Description

<div><p>One day Vasya painted a Cartesian coordinate system on a piece of paper and marked some set of points <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>), (<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>), ..., (<i>x</i><sub class="lower-index"><i>n</i></sub>, <i>y</i><sub class="lower-index"><i>n</i></sub>)</span>. Let's define neighbors for some fixed point from the given set <span class="tex-span">(<i>x</i>, <i>y</i>)</span>: </p><ul> <li> point <span class="tex-span">(<i>x</i>', <i>y</i>')</span> is <span class="tex-span">(<i>x</i>, <i>y</i>)</span>'s right neighbor, if <span class="tex-span"><i>x</i>' &gt; <i>x</i></span> and <span class="tex-span"><i>y</i>' = <i>y</i></span> </li><li> point <span class="tex-span">(<i>x</i>', <i>y</i>')</span> is <span class="tex-span">(<i>x</i>, <i>y</i>)</span>'s left neighbor, if <span class="tex-span"><i>x</i>' &lt; <i>x</i></span> and <span class="tex-span"><i>y</i>' = <i>y</i></span> </li><li> point <span class="tex-span">(<i>x</i>', <i>y</i>')</span> is <span class="tex-span">(<i>x</i>, <i>y</i>)</span>'s lower neighbor, if <span class="tex-span"><i>x</i>' = <i>x</i></span> and <span class="tex-span"><i>y</i>' &lt; <i>y</i></span> </li><li> point <span class="tex-span">(<i>x</i>', <i>y</i>')</span> is <span class="tex-span">(<i>x</i>, <i>y</i>)</span>'s upper neighbor, if <span class="tex-span"><i>x</i>' = <i>x</i></span> and <span class="tex-span"><i>y</i>' &gt; <i>y</i></span> </li></ul><p>We'll consider point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> from the given set supercentral, if it has at least one upper, at least one lower, at least one left and at least one right neighbor among this set's points.</p><p>Vasya marked quite many points on the paper. Analyzing the picture manually is rather a challenge, so Vasya asked you to help him. Your task is to find the number of supercentral points in the given set.</p></div><div class="input-specification"><p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the number of points in the given set. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the points written as "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" (without the quotes) (<span class="tex-span">|<i>x</i>|, |<i>y</i>| ≤ 1000</span>), all coordinates are integers. The numbers in the line are separated by exactly one space. It is guaranteed that all points are different.</p></div><div class="output-specification"><p>Print the only number — the number of supercentral points of the given set.</p></div>

## Input

<p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — the number of points in the given set. Next <span class="tex-span"><i>n</i></span> lines contain the coordinates of the points written as "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" (without the quotes) (<span class="tex-span">|<i>x</i>|, |<i>y</i>| ≤ 1000</span>), all coordinates are integers. The numbers in the line are separated by exactly one space. It is guaranteed that all points are different.</p>

## Output

<p>Print the only number — the number of supercentral points of the given set.</p>





```input1
8
1 1
4 2
3 1
1 2
0 2
0 1
1 0
1 3

```




```input2
5
0 0
0 1
1 0
0 -1
-1 0

```




```output1
2

```




```output2
1

```



## Note

<p>In the first sample the supercentral points are only points <span class="tex-span">(1, 1)</span> and <span class="tex-span">(1, 2)</span>.</p><p>In the second sample there is one supercental point — point <span class="tex-span">(0, 0)</span>.</p>
