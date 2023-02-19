## Description

<div><p>You are given a tree (connected graph without cycles) consisting of $n$ vertices. The tree is unrooted — it is just a connected undirected graph without cycles.</p><p>In one move, you can choose exactly $k$ leaves (leaf is such a vertex that is connected to only one another vertex) connected <span class="tex-font-style-bf">to the same vertex</span> and remove them with edges incident to them. I.e. you choose such leaves $u_1, u_2, \dots, u_k$ that there are edges $(u_1, v)$, $(u_2, v)$, $\dots$, $(u_k, v)$ and remove these leaves and these edges.</p><p>Your task is to find the <span class="tex-font-style-bf">maximum</span> number of moves you can perform if you remove leaves optimally.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $1 \le k &lt; n$) — the number of vertices in the tree and the number of leaves you remove in one move, respectively. The next $n-1$ lines describe edges. The $i$-th edge is represented as two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$), where $x_i$ and $y_i$ are vertices the $i$-th edge connects. It is guaranteed that the given set of edges forms a tree.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>For each test case, print the answer — the <span class="tex-font-style-bf">maximum</span> number of moves you can perform if you remove leaves optimally.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $k$ ($2 \le n \le 2 \cdot 10^5$; $1 \le k &lt; n$) — the number of vertices in the tree and the number of leaves you remove in one move, respectively. The next $n-1$ lines describe edges. The $i$-th edge is represented as two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$), where $x_i$ and $y_i$ are vertices the $i$-th edge connects. It is guaranteed that the given set of edges forms a tree.</p><p>It is guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$).</p>

## Output

<p>For each test case, print the answer — the <span class="tex-font-style-bf">maximum</span> number of moves you can perform if you remove leaves optimally.</p>





```input1
4
8 3
1 2
1 5
7 6
6 8
3 1
6 4
6 1
10 3
1 2
1 10
2 3
1 5
1 6
2 4
7 10
10 9
8 10
7 2
3 1
4 5
3 6
7 4
1 2
1 4
5 1
1 2
2 3
4 3
5 3
```




```output1
2
3
3
4
```



## Note

<p>The picture corresponding to the first test case of the example:</p><p><img class="tex-graphics" src="file://XdaiEqWL.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There you can remove vertices $2$, $5$ and $3$ during the first move and vertices $1$, $7$ and $4$ during the second move.</p><p>The picture corresponding to the second test case of the example:</p><p><img class="tex-graphics" src="file://NR89DeLf.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There you can remove vertices $7$, $8$ and $9$ during the first move, then vertices $5$, $6$ and $10$ during the second move and vertices $1$, $3$ and $4$ during the third move.</p><p>The picture corresponding to the third test case of the example:</p><p><img class="tex-graphics" src="file://SIhpozDj.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There you can remove vertices $5$ and $7$ during the first move, then vertices $2$ and $4$ during the second move and vertices $1$ and $6$ during the third move.</p>
