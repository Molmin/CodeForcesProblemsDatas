## Description

<div><p>Amr loves Geometry. One day he came up with a very interesting problem.</p><p>Amr has a circle of radius <span class="tex-span"><i>r</i></span> and center in point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. He wants the circle center to be in new position <span class="tex-span">(<i>x</i>', <i>y</i>')</span>.</p><p>In one step Amr can put a pin to the border of the circle in a certain point, then rotate the circle around that pin by any angle and finally remove the pin.</p><p>Help Amr to achieve his goal in minimum number of steps.</p></div><div class="input-specification"><p>Input consists of 5 space-separated integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>x</i>'</span> <span class="tex-span"><i>y</i>'</span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i>, <i>y</i>, <i>x</i>', <i>y</i>' ≤ 10<sup class="upper-index">5</sup></span>), circle radius, coordinates of original center of the circle and coordinates of destination center of the circle respectively.</p></div><div class="output-specification"><p>Output a single integer — minimum number of steps required to move the center of the circle to the destination point.</p></div>

## Input

<p>Input consists of 5 space-separated integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>x</i>'</span> <span class="tex-span"><i>y</i>'</span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i>, <i>y</i>, <i>x</i>', <i>y</i>' ≤ 10<sup class="upper-index">5</sup></span>), circle radius, coordinates of original center of the circle and coordinates of destination center of the circle respectively.</p>

## Output

<p>Output a single integer — minimum number of steps required to move the center of the circle to the destination point.</p>





```input1
2 0 0 0 4

```




```input2
1 1 1 4 4

```




```input3
4 5 6 5 6

```




```output1
1

```




```output2
3

```




```output3
0

```



## Note

<p>In the first sample test the optimal way is to put a pin at point <span class="tex-span">(0, 2)</span> and rotate the circle by <span class="tex-span">180</span> degrees counter-clockwise (or clockwise, no matter).</p><p><img class="tex-graphics" src="file://ZP4uEixi.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
