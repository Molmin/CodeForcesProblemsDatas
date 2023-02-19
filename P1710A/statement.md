## Description

<div><p>A picture can be represented as an $n\times m$ grid ($n$ rows and $m$ columns) so that each of the $n \cdot m$ cells is colored with one color. You have $k$ pigments of different colors. You have a limited amount of each pigment, more precisely you can color at most $a_i$ cells with the $i$-th pigment.</p><p>A picture is considered beautiful if each cell has <span class="tex-font-style-bf">at least</span> $3$ <span class="tex-font-style-bf">toroidal</span> neighbors with the same color as itself.</p><p>Two cells are considered <span class="tex-font-style-bf">toroidal</span> neighbors if they <span class="tex-font-style-bf">toroidally</span> share an edge. In other words, for some integers $1 \leq x_1,x_2 \leq n$ and $1 \leq y_1,y_2 \leq m$, the cell in the $x_1$-th row and $y_1$-th column is a toroidal neighbor of the cell in the $x_2$-th row and $y_2$-th column if one of following two conditions holds:</p><ul> <li> $x_1-x_2 \equiv \pm1 \pmod{n}$ and $y_1=y_2$, or </li><li> $y_1-y_2 \equiv \pm1 \pmod{m}$ and $x_1=x_2$. </li></ul><p>Notice that each cell has exactly $4$ toroidal neighbors. For example, if $n=3$ and $m=4$, the toroidal neighbors of the cell $(1, 2)$ (the cell on the first row and second column) are: $(3, 2)$, $(2, 2)$, $(1, 3)$, $(1, 1)$. They are shown in gray on the image below:</p><center> <img class="tex-graphics" src="file://ZadVkVQG.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The gray cells show toroidal neighbors of $(1, 2)$.</span> </center><p>Is it possible to color all cells with the pigments provided and create a beautiful picture?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($3 \leq n,m \leq 10^9$, $1 \leq k \leq 10^5$) — the number of rows and columns of the picture and the number of pigments.</p><p>The next line contains $k$ integers $a_1,a_2,\dots, a_k$ ($1 \leq a_i \leq 10^9$) — $a_i$ is the maximum number of cells that can be colored with the $i$-th pigment.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it is possible to color a beautiful picture. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without quotes).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($3 \leq n,m \leq 10^9$, $1 \leq k \leq 10^5$) — the number of rows and columns of the picture and the number of pigments.</p><p>The next line contains $k$ integers $a_1,a_2,\dots, a_k$ ($1 \leq a_i \leq 10^9$) — $a_i$ is the maximum number of cells that can be colored with the $i$-th pigment.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">Yes</span>" (without quotes) if it is possible to color a beautiful picture. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without quotes).</p>





```input1|2,3,6,7,10,11
6
4 6 3
12 9 8
3 3 2
8 8
3 3 2
9 5
4 5 2
10 11
5 4 2
9 11
10 10 3
11 45 14
```




```output1
Yes
No
Yes
Yes
No
No
```



## Note

<p>In the first test case, one possible solution is as follows:</p><center> <img class="tex-graphics" src="file://qA6oU56K.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the third test case, we can color all cells with pigment $1$.</p>
