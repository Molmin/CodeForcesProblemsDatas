## Description

<div><p>Sam lives in Awesomeburg, its downtown has a triangular shape. Also, the following is true about the triangle:</p><ul> <li> its vertices have integer coordinates, </li><li> the coordinates of vertices are non-negative, and </li><li> its vertices are not on a single line. </li></ul><p>He calls a point on the downtown's border (that is the border of the triangle) <span class="tex-font-style-it">safe</span> if he can reach this point from <span class="tex-font-style-bf">at least one point</span> of the line $y = 0$ walking along some <span class="tex-font-style-bf">straight line</span>, without crossing the interior of the triangle.</p><center> <img class="tex-graphics" src="file://VSWm2wpV.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">In the picture the downtown is marked with grey color. The first path is invalid because it does not go along a straight line. The second path is invalid because it intersects with the interior of the downtown. The third and fourth paths are correct.</span> </center><p>Find the total length of the unsafe parts of the downtown border. It can be proven that these parts are segments and their number is finite.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. Description of the test cases follows.</p><p>Each test case contains three lines, each of them contains two integers $x_i$, $y_i$ ($0 \le x_i, y_i \le 10^9$)&nbsp;— coordinates of the vertices of the downtown's border.</p></div><div class="output-specification"><p>For each test case print a single number&nbsp;— the answer to the problem.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed $10^{-9}$. Formally let your answer be $a$, jury answer be $b$. Your answer will be considered correct if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-9}$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. Description of the test cases follows.</p><p>Each test case contains three lines, each of them contains two integers $x_i$, $y_i$ ($0 \le x_i, y_i \le 10^9$)&nbsp;— coordinates of the vertices of the downtown's border.</p>

## Output

<p>For each test case print a single number&nbsp;— the answer to the problem.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed $10^{-9}$. Formally let your answer be $a$, jury answer be $b$. Your answer will be considered correct if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-9}$.</p>





```input1
5
8 10
10 4
6 2
4 6
0 1
4 2
14 1
11 2
13 2
0 0
4 0
2 4
0 1
1 1
0 0
```




```output1
0.0000000
0
2.0000
0.00
1
```



## Note

<p>In the picture, the downtowns of the first three test cases are illustrated. Triangles are enumerated according to the indices of test cases they belong to.</p><center> <img class="tex-graphics" src="file://LOdEm7y1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the first two test cases, all points on the borders of the downtowns are safe, thus the answers are $0$.</p><p>In the following picture unsafe points for the third test case are marked with black color:</p><center> <img class="tex-graphics" src="file://GOwKxdec.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the fourth test case, all points on the border of the downtown are safe.</p>
