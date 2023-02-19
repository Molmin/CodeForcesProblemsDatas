## Description

<div><p><span class="tex-font-style-it">After being discouraged by 13 time-limit-exceeded verdicts on an ugly geometry problem, you decided to take a relaxing break for arts and crafts.</span></p><p>There is a piece of paper in the shape of a simple polygon with $n$ vertices. The polygon may be non-convex, but we all know that proper origami paper has the property that <span class="tex-font-style-bf">any horizontal line intersects the boundary of the polygon in at most two points.</span></p><p>If you fold the paper along the vertical line $x=f$, what will be the area of the resulting shape? When you fold, the part of the paper to the left of the line is symmetrically reflected on the right side.</p><center> <img class="tex-graphics" src="file://GSj8OgRG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Your task is to answer $q$ independent queries for values $f_1,\ldots,f_q$.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $q$ ($3\le n\le 10^5, 1\le q\le 10^5$) &nbsp;— the number of polygon vertices and queries, respectively.</p><p>Each of the next $n$ lines contains two integers $x_i$, $y_i$ ($|x_i|, |y_i|\le 10^5$) &nbsp;— the coordinates of the $i$-th point of the polygon. The polygon has an edge connecting each pair of adjacent points in the input, and also an edge between $(x_1,y_1)$ and $(x_n,y_n)$. It is guaranteed that the polygon is non-degenerate and that any horizontal line intersects the boundary of the polygon in at most two points. In particular, no boundary edge is strictly horizontal. Two adjacent sides may be collinear.</p><p>Each of the next $q$ lines contains a single integer $f_i$ ($\min\limits_{j=1}^n(x_j)&lt; f_i&lt; \max\limits_{j=1}^n(x_j)$) &nbsp;— the $x$-coordinate of the $i$-th fold query. It is guaranteed that all $f_i$ are distinct.</p></div><div class="output-specification"><p>For each query, output the area $A_i$ of the paper if you fold it along the line $x=f_i$.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-4}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-4}$.</p></div>

## Input

<p>The first line contains two integers $n$, $q$ ($3\le n\le 10^5, 1\le q\le 10^5$) &nbsp;— the number of polygon vertices and queries, respectively.</p><p>Each of the next $n$ lines contains two integers $x_i$, $y_i$ ($|x_i|, |y_i|\le 10^5$) &nbsp;— the coordinates of the $i$-th point of the polygon. The polygon has an edge connecting each pair of adjacent points in the input, and also an edge between $(x_1,y_1)$ and $(x_n,y_n)$. It is guaranteed that the polygon is non-degenerate and that any horizontal line intersects the boundary of the polygon in at most two points. In particular, no boundary edge is strictly horizontal. Two adjacent sides may be collinear.</p><p>Each of the next $q$ lines contains a single integer $f_i$ ($\min\limits_{j=1}^n(x_j)&lt; f_i&lt; \max\limits_{j=1}^n(x_j)$) &nbsp;— the $x$-coordinate of the $i$-th fold query. It is guaranteed that all $f_i$ are distinct.</p>

## Output

<p>For each query, output the area $A_i$ of the paper if you fold it along the line $x=f_i$.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-4}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-4}$.</p>





```input1
4 7
0 10
10 0
0 -10
-10 0
-9
-5
-1
0
1
5
9
```




```input2
4 1
0 0
0 2
2 4
2 2
1
```




```input3
9 4
0 -3
2 -2
-1 -1
0 4
2 5
1 6
-2 3
-1 1
-3 0
0
-2
-1
1
```




```output1
199.0000000000
175.0000000000
119.0000000000
100.0000000000
119.0000000000
175.0000000000
199.0000000000
```




```output2
3.0000000000
```




```output3
11.1250000000
11.7500000000
10.3446969697
11.3333333333
```



## Note

<p>The first test, with the fold $f=-5$:</p><center> <img class="tex-graphics" src="file://i8WuS7ur.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The second test, with the fold $f=1$:</p><center> <img class="tex-graphics" src="file://jcynae20.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The third test, with the fold $f=-1$:</p><center> <img class="tex-graphics" src="file://LiJpCo7A.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
