## Description

<div><p>Little Petya very much likes rectangular tables that consist of characters "0" and "1". Recently he has received one such table as a gift from his mother. The table contained <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. The rows are numbered from top to bottom from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the columns are numbered from the left to the right from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Petya immediately decided to find the longest cool cycle whatever it takes.</p><p>A cycle is a sequence of pairwise distinct cells where each two consecutive cells have a common side; besides, the first cell has a common side with the last cell. A cycle is called cool if it fulfills all the following conditions simultaneously: </p><ul> <li> The cycle entirely consists of the cells that contain "1". </li><li> Each cell that belongs to the cycle, has a common side with exactly two other cells that belong to the cycle. </li><li> Each cell of the table that contains "1" either belongs to the cycle or is positioned outside of it (see definition below). </li></ul><p>To define the notion of "outside" formally, let's draw a cycle on a plane. Let each cell of the cycle <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span"><i>i</i></span> is the row number, <span class="tex-span"><i>j</i></span> is the column number) correspond to the point <span class="tex-span">(<i>i</i>, <i>j</i>)</span> on the coordinate plane. Let a straight line segment join each pair of points that correspond to the cells belonging to the cycle and sharing a side. Thus, we will get a closed polyline that has no self-intersections and self-touches. The polyline divides the plane into two connected parts: the part of an infinite area and the part of a finite area. It is considered that cell <span class="tex-span">(<i>r</i>, <i>c</i>)</span> lies outside of the cycle if it does not belong to the cycle and the corresponding point on the plane with coordinates <span class="tex-span">(<i>r</i>, <i>c</i>)</span> lies in the part with the infinite area.</p><p>Help Petya to find the length of the longest cool cycle in the table. The cycle length is defined as the number of cells that belong to the cycle.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of rows and columns in the table, respectively. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. Each character can be either "0" or "1".</p></div><div class="output-specification"><p>Print a single number — the length of the longest cool cycle in the table. If such cycles do not exist, print 0.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) — the number of rows and columns in the table, respectively. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters. Each character can be either "0" or "1".</p>

## Output

<p>Print a single number — the length of the longest cool cycle in the table. If such cycles do not exist, print 0.</p>





```input1
3 3
111
101
111

```




```input2
5 5
01010
10101
01010
10101
01010

```




```input3
7 7
1111111
1000101
1000101
1000101
1000111
1000001
1111111

```




```input4
5 5
11111
10001
10101
10001
11111

```




```output1
8

```




```output2
0

```




```output3
24

```




```output4
0

```



## Note

<p>In the first example there's only one cycle and it is cool.</p><p>In the second sample there's no cycle at all.</p><p>In the third sample there are two cool cycles: their lengths are 12 and 24.</p><p>In the fourth sample there also is only one cycle but it isn't cool as there's a cell containing "1" inside this cycle.</p>
