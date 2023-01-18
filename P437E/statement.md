## Description

<div><p>This time our child has a simple polygon. He has to find the number of ways to split the polygon into non-degenerate triangles, each way must satisfy the following requirements:</p><ul> <li> each vertex of each triangle is one of the polygon vertex; </li><li> each side of the polygon must be the side of exactly one triangle; </li><li> the area of intersection of every two triangles equals to zero, and the sum of all areas of triangles equals to the area of the polygon; </li><li> each triangle must be completely inside the polygon; </li><li> <span class="tex-font-style-bf">each side of each triangle must contain exactly two vertices of the polygon</span>. </li></ul><p>The picture below depicts an example of a correct splitting.</p><center> <img class="tex-graphics" src="file://StBb4hz8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Please, help the child. Calculate the described number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup>  +  7)</span> for him.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 200)</span> — the number of vertices of the polygon. Then follow <span class="tex-span"><i>n</i></span> lines, each line containing two integers. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">7</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th vertex of the polygon in clockwise or counterclockwise order.</p><p>It's guaranteed that the polygon is simple.</p></div><div class="output-specification"><p>Output the number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup>  +  7)</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 200)</span> — the number of vertices of the polygon. Then follow <span class="tex-span"><i>n</i></span> lines, each line containing two integers. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">7</sup>)</span> — the <span class="tex-span"><i>i</i></span>-th vertex of the polygon in clockwise or counterclockwise order.</p><p>It's guaranteed that the polygon is simple.</p>

## Output

<p>Output the number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup>  +  7)</span>.</p>





```input1
4
0 0
0 1
1 1
1 0

```




```input2
4
0 0
1 0
0 1
-1 0

```




```input3
5
0 0
1 0
1 1
0 1
-2 -1

```




```output1
2

```




```output2
1

```




```output3
3

```



## Note

<p>In the first sample, there are two possible splittings:</p><center> <img class="tex-graphics" src="file://0vr1vSL6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, there are only one possible splitting:</p><center> <img class="tex-graphics" src="file://ANPXNoou.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
