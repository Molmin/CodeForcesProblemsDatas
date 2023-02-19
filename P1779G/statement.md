## Description

<div><p>The time has finally come, MKnez and Baltic are to host <span class="tex-font-style-it">The Game of the Century</span>. For that purpose, they built a village to lodge its participants.</p><p>The village has the shape of an equilateral triangle delimited by three roads of length $n$. It is cut into $n^2$ smaller equilateral triangles, of side length $1$, by $3n-3$ additional roads which run parallel to the sides. See the figure for $n=3$. Each of the $3n$ roads is made of multiple (possibly $1$) road segments of length $1$ which connect adjacent intersections.</p><center> <img class="tex-graphics" src="file://A3KPggiY.png" style="max-width: 100.0%;max-height: 100.0%;">   </center><p>The direction has already been chosen for each of the $3n$ roads (so, for each road, the same direction is assigned to all its road segments). Traffic can only go in the specified directions (i.&nbsp;e. the roads are monodirectional).</p><p>You are tasked with making adjustments to the traffic plan so that from each intersection it is possible to reach every other intersection. Specifically, you can invert the traffic direction of any number of road segments of length $1$. What is the minimal number of road segments for which you need to invert the traffic direction?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a positive integer $n$ ($1\leq n\leq 10^5$) &nbsp;— the size of the triangular village's sides.</p><p>Three lines follow, each containing a binary string of length $n$ which describes the traffic directions of the roads. </p><p>The $i$-th of the following three lines contains a binary string $s_i$ of length $n$ representing the direction of each road parallel to the road segment denoted by $i$ in the picture above. In particular, the $j$-th character of $s_i$ is "<span class="tex-font-style-tt">1</span>" if the $j$-th shortest road (parallel to the road segment denoted by $i$ in the picture) has the same direction of the road segment denoted by $i$ in the picture, while it is "<span class="tex-font-style-tt">0</span>" if it has the opposite direction. So the first character of $s_i$ describes the direction of the road containing only $1$ road segment, while the last character describes the direction of the road containing $n$ road segments.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the minimum number of road segments for which you need to invert the traffic direction.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a positive integer $n$ ($1\leq n\leq 10^5$) &nbsp;— the size of the triangular village's sides.</p><p>Three lines follow, each containing a binary string of length $n$ which describes the traffic directions of the roads. </p><p>The $i$-th of the following three lines contains a binary string $s_i$ of length $n$ representing the direction of each road parallel to the road segment denoted by $i$ in the picture above. In particular, the $j$-th character of $s_i$ is "<span class="tex-font-style-tt">1</span>" if the $j$-th shortest road (parallel to the road segment denoted by $i$ in the picture) has the same direction of the road segment denoted by $i$ in the picture, while it is "<span class="tex-font-style-tt">0</span>" if it has the opposite direction. So the first character of $s_i$ describes the direction of the road containing only $1$ road segment, while the last character describes the direction of the road containing $n$ road segments.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print the minimum number of road segments for which you need to invert the traffic direction.</p>





```input1|2,3,4,5,10,11,12,13
3
3
001
001
010
1
0
0
0
3
111
011
100
```




```output1
2
0
3
```



## Note

<p>The first example corresponds to the picture in the statement. There exist multiple solutions that invert the traffic direction of exactly $2$ road segments, but inverting only $1$ road segment never makes it possible to reach every intersection from any other. One of the possible solutions is shown in the picture below in which the inverted road segments are highlighted in blue.</p><center> <img class="tex-graphics" src="file://feC7uMMi.png" style="max-width: 100.0%;max-height: 100.0%;">   </center><p>In the second example, the answer is $0$ since it is already possible to reach every intersection from any other.</p>
