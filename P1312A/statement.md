## Description

<div><p>You are given two integers $n$ and $m$ ($m &lt; n$). Consider a <span class="tex-font-style-bf">convex</span> regular polygon of $n$ vertices. Recall that a regular polygon is a polygon that is equiangular (all angles are equal in measure) and equilateral (all sides have the same length).</p><center> <img class="tex-graphics" src="file://HRgugiwL.png" style="max-width: 100.0%;max-height: 100.0%;"> Examples of convex regular polygons </center><p>Your task is to say if it is possible to build another <span class="tex-font-style-bf">convex</span> regular polygon with $m$ vertices such that its center coincides with the center of the initial polygon and each of its vertices is some vertex of the initial polygon.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The next $t$ lines describe test cases. Each test case is given as two space-separated integers $n$ and $m$ ($3 \le m &lt; n \le 100$) — the number of vertices in the initial polygon and the number of vertices in the polygon you want to build.</p></div><div class="output-specification"><p>For each test case, print the answer — "<span class="tex-font-style-tt">YES</span>" (without quotes), if it is possible to build another <span class="tex-font-style-bf">convex</span> regular polygon with $m$ vertices such that its center coincides with the center of the initial polygon and each of its vertices is some vertex of the initial polygon and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The next $t$ lines describe test cases. Each test case is given as two space-separated integers $n$ and $m$ ($3 \le m &lt; n \le 100$) — the number of vertices in the initial polygon and the number of vertices in the polygon you want to build.</p>

## Output

<p>For each test case, print the answer — "<span class="tex-font-style-tt">YES</span>" (without quotes), if it is possible to build another <span class="tex-font-style-bf">convex</span> regular polygon with $m$ vertices such that its center coincides with the center of the initial polygon and each of its vertices is some vertex of the initial polygon and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
2
6 3
7 3
```




```output1
YES
NO
```



## Note

<center> <img class="tex-graphics" src="file://H8jjWAhq.png" style="max-width: 100.0%;max-height: 100.0%;"> The first test case of the example </center><p>It can be shown that the answer for the second test case of the example is "<span class="tex-font-style-tt">NO</span>".</p>
