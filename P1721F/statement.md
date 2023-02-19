## Description

<div><p>You are given a bipartite graph with $n_1$ vertices in the first part, $n_2$ vertices in the second part, and $m$ edges. The maximum matching in this graph is the maximum possible (by size) subset of edges of this graph such that no vertex is incident to more than one chosen edge.</p><p>You have to process two types of queries to this graph:</p><ul> <li> $1$ — remove the <span class="tex-font-style-bf">minimum possible</span> number of vertices from this graph so that the size of the maximum matching gets reduced <span class="tex-font-style-bf">exactly by $1$</span>, and print the vertices that you have removed. Then, find any maximum matching in this graph and print the sum of indices of edges belonging to this matching; </li><li> $2$ — query of this type will be asked only after a query of type $1$. As the answer to this query, you have to print the edges forming the maximum matching you have chosen in the previous query. </li></ul><p>Note that you should solve the problem in <span class="tex-font-style-tt">online</span> mode. It means that you can't read the whole input at once. You can read each query only after writing the answer for the last query. Use functions <span class="tex-font-style-tt">fflush</span> in <span class="tex-font-style-tt">C++</span> and <span class="tex-font-style-tt">BufferedWriter.flush</span> in <span class="tex-font-style-tt">Java</span> languages after each writing in your program.</p></div><div class="input-specification"><p>The first line contains four integers $n_1$, $n_2$, $m$ and $q$ ($1 \le n_1, n_2 \le 2 \cdot 10^5$; $1 \le m \le \min(n_1 \cdot n_2, 2 \cdot 10^5)$; $1 \le q \le 2 \cdot 10^5$).</p><p>Then $m$ lines follow. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n_1$; $1 \le y_i \le n_2$) meaning that the $i$-th edge connects the vertex $x_i$ in the first part and the vertex $y_i$ in the second part. There are no pairs of vertices that are connected by more than one edge.</p><p>Then $q$ lines follow. The $i$-th of them contains one integer, $1$ or $2$, denoting the $i$-th query. Additional constraints on queries:</p><ul> <li> the number of queries of type $1$ won't exceed the size of the maximum matching in the initial graph; </li><li> the number of queries of type $2$ won't exceed $3$; </li><li> each query of type $2$ is preceded by a query of type $1$; </li><li> your solution is allowed to read the $i$-th query only after printing the answer for the $(i-1)$-th query and flushing the output. </li></ul></div><div class="output-specification"><p>For a query of type $1$, print the answer in three lines as follows:</p><ul> <li> the first line should contain the number of vertices you remove; </li><li> the second line should contain the indices of vertices you remove, as follows: if you remove the vertex $x$ from the left part, print $x$; if you remove the vertex $y$ from the right part, print $-y$ (negative index); </li><li> the third line should contain the sum of indices of edges in some maximum matching in the resulting graph. The edges are numbered from $1$ to $m$. </li></ul><p>For a query of type $2$, print the answer in two lines as follows:</p><ul> <li> the first line should contain the size of the maximum matching; </li><li> the second line should contain the indices of the edges belonging to the maximum matching. Note that the sum of these indices should be equal to the number you printed at the end of the previous query of type $1$; </li></ul><p>After printing the answer to a query, don't forget to flush the output.</p></div>

## Input

<p>The first line contains four integers $n_1$, $n_2$, $m$ and $q$ ($1 \le n_1, n_2 \le 2 \cdot 10^5$; $1 \le m \le \min(n_1 \cdot n_2, 2 \cdot 10^5)$; $1 \le q \le 2 \cdot 10^5$).</p><p>Then $m$ lines follow. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n_1$; $1 \le y_i \le n_2$) meaning that the $i$-th edge connects the vertex $x_i$ in the first part and the vertex $y_i$ in the second part. There are no pairs of vertices that are connected by more than one edge.</p><p>Then $q$ lines follow. The $i$-th of them contains one integer, $1$ or $2$, denoting the $i$-th query. Additional constraints on queries:</p><ul> <li> the number of queries of type $1$ won't exceed the size of the maximum matching in the initial graph; </li><li> the number of queries of type $2$ won't exceed $3$; </li><li> each query of type $2$ is preceded by a query of type $1$; </li><li> your solution is allowed to read the $i$-th query only after printing the answer for the $(i-1)$-th query and flushing the output. </li></ul>

## Output

<p>For a query of type $1$, print the answer in three lines as follows:</p><ul> <li> the first line should contain the number of vertices you remove; </li><li> the second line should contain the indices of vertices you remove, as follows: if you remove the vertex $x$ from the left part, print $x$; if you remove the vertex $y$ from the right part, print $-y$ (negative index); </li><li> the third line should contain the sum of indices of edges in some maximum matching in the resulting graph. The edges are numbered from $1$ to $m$. </li></ul><p>For a query of type $2$, print the answer in two lines as follows:</p><ul> <li> the first line should contain the size of the maximum matching; </li><li> the second line should contain the indices of the edges belonging to the maximum matching. Note that the sum of these indices should be equal to the number you printed at the end of the previous query of type $1$; </li></ul><p>After printing the answer to a query, don't forget to flush the output.</p>





```input1
3 4 4 4
2 2
1 3
2 1
3 4
1
2
1
2
```




```output1
1
-4
3
===
2
1 2
===
1
2
2
===
1
2
```



## Note

<p>In this problem, you may receive the verdict "Idleness Limit Exceeded" since it is in online mode. If it happens, it means that either the output format is wrong, or you don't meet some constraint of the problem. You may treat this verdict as "Wrong Answer".</p><p>For your convenience, the output for queries in the example is separated by the line <span class="tex-font-style-tt">===</span>. <span class="tex-font-style-bf">Don't print this line in your program, it is done only to make sure that it's easy to distinguish between answers for different queries in the statement</span>.</p>
