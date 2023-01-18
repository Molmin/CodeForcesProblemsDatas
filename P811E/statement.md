## Description

<div><p>In his spare time Vladik estimates beauty of the flags.</p><p>Every flag could be represented as the matrix <span class="tex-span"><i>n</i> × <i>m</i></span> which consists of positive integers.</p><p>Let's define the beauty of the flag as number of components in its matrix. We call component a set of cells with same numbers and between any pair of cells from that set there exists a path through adjacent cells from same component. Here is the example of the partitioning some flag matrix into components:</p><center> <img class="tex-graphics" src="file://OUuGKmlU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>But this time he decided to change something in the process. Now he wants to estimate not the entire flag, but some segment. Segment of flag can be described as a submatrix of the flag matrix with opposite corners at <span class="tex-span">(1, <i>l</i>)</span> and <span class="tex-span">(<i>n</i>, <i>r</i>)</span>, where conditions <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>m</i></span> are satisfied.</p><p>Help Vladik to calculate the beauty for some segments of the given flag.</p></div><div class="input-specification"><p>First line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— dimensions of flag matrix and number of segments respectively.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> space-separated integers&nbsp;— description of flag matrix. All elements of flag matrix is positive integers not exceeding <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains two space-separated integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>m</i></span>)&nbsp;— borders of segment which beauty Vladik wants to know.</p></div><div class="output-specification"><p>For each segment print the result on the corresponding line.</p></div>

## Input

<p>First line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— dimensions of flag matrix and number of segments respectively.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> space-separated integers&nbsp;— description of flag matrix. All elements of flag matrix is positive integers not exceeding <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contains two space-separated integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>m</i></span>)&nbsp;— borders of segment which beauty Vladik wants to know.</p>

## Output

<p>For each segment print the result on the corresponding line.</p>





```input1
4 5 4
1 1 1 1 1
1 2 2 3 3
1 1 1 2 5
4 4 5 5 5
1 5
2 5
1 2
4 5

```




```output1
6
7
3
4

```



## Note

<p>Partitioning on components for every segment from first test case:</p><p><img class="tex-graphics" src="file://iSuZdkuC.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
