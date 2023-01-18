## Description

<div><p>On the coordinate plane there is a square with sides parallel to the coordinate axes. The length of the square side is equal to <span class="tex-span"><i>a</i></span>. The lower left corner of the square coincides with the point (<span class="tex-span">0, 0</span>) (the point of the origin). The upper right corner of the square has positive coordinates.</p><p>You are given a point with coordinates (<span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>). Your task is to determine whether this point is located strictly inside the square, on its side, or strictly outside the square.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 1000</span>, <span class="tex-span"> - 1000 ≤ <i>x</i>, <i>y</i> ≤ 1000</span>) — the length of the square side and the coordinates of the point which should be checked.</p></div><div class="output-specification"><p>Print one integer:</p><ul> <li> 0, if the point is located strictly inside the square; </li><li> 1, if the point is located on the side of the square; </li><li> 2, if the point is located strictly outside the square. </li></ul></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 1000</span>, <span class="tex-span"> - 1000 ≤ <i>x</i>, <i>y</i> ≤ 1000</span>) — the length of the square side and the coordinates of the point which should be checked.</p>

## Output

<p>Print one integer:</p><ul> <li> 0, if the point is located strictly inside the square; </li><li> 1, if the point is located on the side of the square; </li><li> 2, if the point is located strictly outside the square. </li></ul>





```input1
2 1 1

```




```input2
4 4 4

```




```input3
10 5 -4

```




```output1
0

```




```output2
1

```




```output3
2

```


