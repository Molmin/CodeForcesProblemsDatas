## Description

<div><p>You are given $m$ sets of integers $A_1, A_2, \ldots, A_m$; elements of these sets are integers between $1$ and $n$, inclusive.</p><p>There are two arrays of positive integers $a_1, a_2, \ldots, a_m$ and $b_1, b_2, \ldots, b_n$. </p><p>In one operation you can delete an element $j$ from the set $A_i$ and pay $a_i + b_j$ coins for that.</p><p>You can make several (maybe none) operations (some sets can become empty).</p><p>After that, you will make an edge-colored undirected graph consisting of $n$ vertices. For each set $A_i$ you will add an edge $(x, y)$ with color $i$ for all $x, y \in A_i$ and $x &lt; y$. Some pairs of vertices can be connected with more than one edge, but such edges have different colors.</p><p>You call a cycle $i_1 \to e_1 \to i_2 \to e_2 \to \ldots \to i_k \to e_k \to i_1$ ($e_j$ is some edge connecting vertices $i_j$ and $i_{j+1}$ in this graph) <span class="tex-font-style-it">rainbow</span> if all edges on it have different colors.</p><p>Find the minimum number of coins you should pay to get a graph without rainbow cycles.</p></div><div class="input-specification"><p>The first line contains two integers $m$ and $n$ ($1 \leq m, n \leq 10^5$), the number of sets and the number of vertices in the graph.</p><p>The second line contains $m$ integers $a_1, a_2, \ldots, a_m$ ($1 \leq a_i \leq 10^9$).</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^9$).</p><p>In the each of the next of $m$ lines there are descriptions of sets. In the $i$-th line the first integer $s_i$ ($1 \leq s_i \leq n$) is equal to the size of $A_i$. Then $s_i$ integers follow: the elements of the set $A_i$. These integers are from $1$ to $n$ and distinct.</p><p>It is guaranteed that the sum of $s_i$ for all $1 \leq i \leq m$ does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print one integer: the minimum number of coins you should pay for operations to avoid rainbow cycles in the obtained graph.</p></div>

## Input

<p>The first line contains two integers $m$ and $n$ ($1 \leq m, n \leq 10^5$), the number of sets and the number of vertices in the graph.</p><p>The second line contains $m$ integers $a_1, a_2, \ldots, a_m$ ($1 \leq a_i \leq 10^9$).</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^9$).</p><p>In the each of the next of $m$ lines there are descriptions of sets. In the $i$-th line the first integer $s_i$ ($1 \leq s_i \leq n$) is equal to the size of $A_i$. Then $s_i$ integers follow: the elements of the set $A_i$. These integers are from $1$ to $n$ and distinct.</p><p>It is guaranteed that the sum of $s_i$ for all $1 \leq i \leq m$ does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print one integer: the minimum number of coins you should pay for operations to avoid rainbow cycles in the obtained graph.</p>





```input1
3 2
1 2 3
4 5
2 1 2
2 1 2
2 1 2
```




```input2
7 8
3 6 7 9 10 7 239
8 1 9 7 10 2 6 239
3 2 1 3
2 4 1
3 1 3 7
2 4 3
5 3 4 5 6 7
2 5 7
1 8
```




```output1
11
```




```output2
66
```



## Note

<p>In the first test, you can make such operations:</p><ul> <li> Delete element $1$ from set $1$. You should pay $a_1 + b_1 = 5$ coins for that. </li><li> Delete element $1$ from set $2$. You should pay $a_2 + b_1 = 6$ coins for that. </li></ul><p>You pay $11$ coins in total. After these operations, the first and the second sets will be equal to $\{2\}$ and the third set will be equal to $\{1, 2\}$.</p><p>So, the graph will consist of one edge $(1, 2)$ of color $3$.</p><p>In the second test, you can make such operations:</p><ul> <li> Delete element $1$ from set $1$. You should pay $a_1 + b_1 = 11$ coins for that. </li><li> Delete element $4$ from set $2$. You should pay $a_2 + b_4 = 13$ coins for that. </li><li> Delete element $7$ from set $3$. You should pay $a_3 + b_7 = 13$ coins for that. </li><li> Delete element $4$ from set $4$. You should pay $a_4 + b_4 = 16$ coins for that. </li><li> Delete element $7$ from set $6$. You should pay $a_6 + b_7 = 13$ coins for that. </li></ul><p>You pay $66$ coins in total.</p><p>After these operations, the sets will be:</p><ul> <li> $\{2, 3\}$; </li><li> $\{1\}$; </li><li> $\{1, 3\}$; </li><li> $\{3\}$; </li><li> $\{3, 4, 5, 6, 7\}$; </li><li> $\{5\}$; </li><li> $\{8\}$. </li></ul><p>We will get the graph:</p><p><img class="tex-graphics" src="file://dC5nPtMM.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>There are no rainbow cycles in it.</p>
