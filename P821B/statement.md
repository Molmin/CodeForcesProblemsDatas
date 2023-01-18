## Description

<div><p>Okabe needs bananas for one of his experiments for some strange reason. So he decides to go to the forest and cut banana trees.</p><p>Consider the point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> in the 2D plane such that <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are integers and <span class="tex-span">0 ≤ <i>x</i>, <i>y</i></span>. There is a tree in such a point, and it has <span class="tex-span"><i>x</i> + <i>y</i></span> bananas. There are no trees nor bananas in other points. Now, Okabe draws a line with equation <img align="middle" class="tex-formula" src="file://S2PFW1XI.png" style="max-width: 100.0%;max-height: 100.0%;">. Okabe can select a single rectangle with axis aligned sides with all points on or under the line and cut all the trees in all points that are inside or on the border of this rectangle and take their bananas. Okabe's rectangle can be degenerate; that is, it can be a line segment or even a point.</p><p>Help Okabe and find the maximum number of bananas he can get if he chooses the rectangle wisely.</p><p>Okabe is sure that the answer does not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>. You can trust him.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10000</span>).</p></div><div class="output-specification"><p>Print the maximum number of bananas Okabe can get from the trees he cuts.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>b</i> ≤ 10000</span>).</p>

## Output

<p>Print the maximum number of bananas Okabe can get from the trees he cuts.</p>





```input1
1 5

```




```input2
2 3

```




```output1
30

```




```output2
25

```



## Note

<center> <img class="tex-graphics" src="file://OMFo8G27.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The graph above corresponds to sample test 1. The optimal rectangle is shown in red and has <span class="tex-span">30</span> bananas.</p>
