## Description

<div><p>You are given a tree with $n$ vertices. You are allowed to modify the structure of the tree through the following multi-step operation:</p><ol> <li> Choose three vertices $a$, $b$, and $c$ such that $b$ is adjacent to both $a$ and $c$. </li><li> For every vertex $d$ <span class="tex-font-style-bf">other than $b$</span> that is adjacent to $a$, remove the edge connecting $d$ and $a$ and add the edge connecting $d$ and $c$. </li><li> Delete the edge connecting $a$ and $b$ and add the edge connecting $a$ and $c$. </li></ol><p>As an example, consider the following tree:</p><center> <img class="tex-graphics" src="file://fekY7fPm.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The following diagram illustrates the sequence of steps that happen when we apply an operation to vertices $2$, $4$, and $5$:</p><center> <img class="tex-graphics" src="file://ZyKRZBpk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It can be proven that after each operation, the resulting graph is still a tree.</p><p>Find the minimum number of operations that must be performed to transform the tree into a star. A star is a tree with one vertex of degree $n - 1$, called its center, and $n - 1$ vertices of degree $1$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \le n \le 2 \cdot 10^5$) &nbsp;— the number of vertices in the tree.</p><p>The $i$-th of the following $n - 1$ lines contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$) denoting that there exists an edge connecting vertices $u_i$ and $v_i$. It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>Print a single integer &nbsp;— the minimum number of operations needed to transform the tree into a star.</p><p>It can be proven that under the given constraints, it is always possible to transform the tree into a star using at most $10^{18}$ operations.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \le n \le 2 \cdot 10^5$) &nbsp;— the number of vertices in the tree.</p><p>The $i$-th of the following $n - 1$ lines contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$, $u_i \neq v_i$) denoting that there exists an edge connecting vertices $u_i$ and $v_i$. It is guaranteed that the given edges form a tree.</p>

## Output

<p>Print a single integer &nbsp;— the minimum number of operations needed to transform the tree into a star.</p><p>It can be proven that under the given constraints, it is always possible to transform the tree into a star using at most $10^{18}$ operations.</p>





```input1
6
4 5
2 6
3 2
1 2
2 4
```




```input2
4
2 4
4 1
3 4
```




```output1
1
```




```output2
0
```



## Note

<p>The first test case corresponds to the tree shown in the statement. As we have seen before, we can transform the tree into a star with center at vertex $5$ by applying a single operation to vertices $2$, $4$, and $5$.</p><p>In the second test case, the given tree is already a star with the center at vertex $4$, so no operations have to be performed.</p>
