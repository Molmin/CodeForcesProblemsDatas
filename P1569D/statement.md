## Description

<div><p>There is a city that can be represented as a square grid with corner points in $(0, 0)$ and $(10^6, 10^6)$.</p><p>The city has $n$ vertical and $m$ horizontal streets that goes across the whole city, i.&nbsp;e. the $i$-th vertical streets goes from $(x_i, 0)$ to $(x_i, 10^6)$ and the $j$-th horizontal street goes from $(0, y_j)$ to $(10^6, y_j)$. </p><p>All streets are bidirectional. Borders of the city are streets as well.</p><p>There are $k$ persons staying <span class="tex-font-style-it">on the streets</span>: the $p$-th person at point $(x_p, y_p)$ (so either $x_p$ equal to some $x_i$ or $y_p$ equal to some $y_j$, or both).</p><p>Let's say that a pair of persons form an <span class="tex-font-style-it">inconvenient pair</span> if the shortest path from one person to another going only by streets is <span class="tex-font-style-it">strictly greater</span> than the Manhattan distance between them.</p><p>Calculate the number of inconvenient pairs of persons (pairs $(x, y)$ and $(y, x)$ are the same pair).</p><p>Let's recall that Manhattan distance between points $(x_1, y_1)$ and $(x_2, y_2)$ is $|x_1 - x_2| + |y_1 - y_2|$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$ and $k$ ($2 \le n, m \le 2 \cdot 10^5$; $2 \le k \le 3 \cdot 10^5$)&nbsp;— the number of vertical and horizontal streets and the number of persons.</p><p>The second line of each test case contains $n$ integers $x_1, x_2, \dots, x_n$ ($0 = x_1 &lt; x_2 &lt; \dots &lt; x_{n - 1} &lt; x_n = 10^6$)&nbsp;— the $x$-coordinates of vertical streets.</p><p>The third line contains $m$ integers $y_1, y_2, \dots, y_m$ ($0 = y_1 &lt; y_2 &lt; \dots &lt; y_{m - 1} &lt; y_m = 10^6$)&nbsp;— the $y$-coordinates of horizontal streets.</p><p>Next $k$ lines contains description of people. The $p$-th line contains two integers $x_p$ and $y_p$ ($0 \le x_p, y_p \le 10^6$; $x_p \in \{x_1, \dots, x_n\}$ or $y_p \in \{y_1, \dots, y_m\}$)&nbsp;— the coordinates of the $p$-th person. All points are distinct.</p><p>It guaranteed that sum of $n$ doesn't exceed $2 \cdot 10^5$, sum of $m$ doesn't exceed $2 \cdot 10^5$ and sum of $k$ doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the number of inconvenient pairs.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$ and $k$ ($2 \le n, m \le 2 \cdot 10^5$; $2 \le k \le 3 \cdot 10^5$)&nbsp;— the number of vertical and horizontal streets and the number of persons.</p><p>The second line of each test case contains $n$ integers $x_1, x_2, \dots, x_n$ ($0 = x_1 &lt; x_2 &lt; \dots &lt; x_{n - 1} &lt; x_n = 10^6$)&nbsp;— the $x$-coordinates of vertical streets.</p><p>The third line contains $m$ integers $y_1, y_2, \dots, y_m$ ($0 = y_1 &lt; y_2 &lt; \dots &lt; y_{m - 1} &lt; y_m = 10^6$)&nbsp;— the $y$-coordinates of horizontal streets.</p><p>Next $k$ lines contains description of people. The $p$-th line contains two integers $x_p$ and $y_p$ ($0 \le x_p, y_p \le 10^6$; $x_p \in \{x_1, \dots, x_n\}$ or $y_p \in \{y_1, \dots, y_m\}$)&nbsp;— the coordinates of the $p$-th person. All points are distinct.</p><p>It guaranteed that sum of $n$ doesn't exceed $2 \cdot 10^5$, sum of $m$ doesn't exceed $2 \cdot 10^5$ and sum of $k$ doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print the number of inconvenient pairs.</p>





```input1
2
2 2 4
0 1000000
0 1000000
1 0
1000000 1
999999 1000000
0 999999
5 4 9
0 1 2 6 1000000
0 4 8 1000000
4 4
2 5
2 2
6 3
1000000 1
3 8
5 8
8 8
6 8
```




```output1
2
5
```



## Note

<p>The second test case is pictured below: </p><center> <img class="tex-graphics" src="file://3aBkNnpD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For example, points $3$ and $4$ form an inconvenient pair, since the shortest path between them (shown red and equal to $7$) is greater than its Manhattan distance (equal to $5$).</p><p>Points $3$ and $5$ also form an inconvenient pair: the shortest path equal to $1000001$ (shown green) is greater than the Manhattan distance equal to $999999$.</p><p>But points $5$ and $9$ don't form an inconvenient pair, since the shortest path (shown purple) is equal to its Manhattan distance.</p>
