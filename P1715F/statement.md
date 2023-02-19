## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Farmer Stanley grows corn on a rectangular field of size $ n \times m $ meters with corners in points $(0, 0)$, $(0, m)$, $(n, 0)$, $(n, m)$. This year the harvest was plentiful and corn covered the whole field.</p><p>The night before harvest aliens arrived and poisoned the corn in a single $1 \times 1$ square with sides parallel to field borders. The corn inside the square must not be eaten, but you cannot distinguish it from ordinary corn by sight. Stanley can only collect a sample of corn from an arbitrary polygon and bring it to the laboratory, where it will be analyzed and Stanley will be told the amount of corn in the sample that was poisoned. Since the harvest will soon deteriorate, such a study can be carried out no more than $5$ times.</p><p>More formally, it is allowed to make no more than $5$ queries, each of them calculates the area of intersection of a chosen polygon with a square of poisoned corn. It is necessary to find out the coordinates of the lower-left corner of the drawn square (the vertex of the square with the smallest $x$ and $y$ coordinates).</p></div><div class="input-specification"><p>First line contains two integers $n$ and $m$ ($1 \le n, m \le 100$)&nbsp;— field sizes.</p></div><div><h2>Interaction</h2><p>In order to query the area of intersection of a polygon with $k$ ($3 \le k \le 1000$) vertices at points with coordinates $(x_1, y_1),\; \dots ,\;(x_k, y_k)$ with a square of poisoned corn print $k+1$ lines. In the first of these lines print "<span class="tex-font-style-tt">? k</span>". In the $i$-th of the next $k$ lines print two real numbers $x_i$ and $y_i$ ($|x_i|, |y_i| \le 10^4$) with at most $15$ digits after decimal place.</p><p>The polygon must have <span class="tex-font-style-bf">strictly positive area</span> and contain <span class="tex-font-style-bf">no self-intersections</span>.</p><p>In response to this query you will receive a real number $s$ ($0 \le s \le 1$) with $15$ digits after decimal place&nbsp;— the area of intersection of the square with the given polygon. If the polygon is invalid, there is no guarantee on the valid response.</p><p>When you have identified the drawn square, print on a separate line "<span class="tex-font-style-tt">! x y</span>", where $x$ and $y$ are real numbers with at most $15$ digits after decimal place representing the coordinates of its lower-left corner ($0 \le x \le n - 1$, $0 \le y \le m - 1$), and then you have to terminate your program.</p><p>Your answer will be considered correct if its absolute or relative error on both coordinates does not exceed $10^{-6}$. Formally let your answer be $a$, jury answer be $b$. Your answer will be considered correct if $\frac{|a-b|}{max(1,|b|)} \le 10^{-6}$.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To make a hack, use the following test format.</p><p>The first line of the input should contain two integers $n$ and $m$ ($1 \le n,m \le 100$)&nbsp;— field sizes.</p><p>The second line should contain two real numbers $x$ ($0 \le x \le n - 1$) and $y$ ($0 \le y \le m - 1$)&nbsp;— coordinates of the lower-left corner of the square of poisoned corn.</p></div>

## Input

<p>First line contains two integers $n$ and $m$ ($1 \le n, m \le 100$)&nbsp;— field sizes.</p>





```input1
3 3





0.5





0.5
```




```output1
? 4
0 0
2 0
2 3
0 3

? 4
0 0
0 1
3 1
3 0

! 1.5 0.5
```



## Note

<p>In the first test from the statement, the aliens poisoned a square of corn with vertices at points with coordinates $(1.5, 0.5)$, $(1.5, 1.5)$, $(2.5, 1.5)$, $(2.5, 0.5)$. In the picture, it is red, the polygon selected in the query is blue, and their intersection is green.</p><p>Picture for the first query:</p><center> <img class="tex-graphics" height="151px" src="file://t0mHzjVT.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Picture for the second query:</p><center> <img class="tex-graphics" height="151px" src="file://mMBNhKmM.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
