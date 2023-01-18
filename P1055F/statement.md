## Description

<div><p>You are given a connected undirected graph without cycles (that is, a tree) of $n$ vertices, moreover, there is a non-negative integer written on every edge.</p><p>Consider all pairs of vertices $(v, u)$ (that is, there are exactly $n^2$ such pairs) and for each pair calculate the bitwise exclusive or (<span class="tex-font-style-tt">xor</span>) of all integers on edges of the simple path between $v$ and $u$. If the path consists of one vertex only, then xor of all integers on edges of this path is equal to $0$.</p><p>Suppose we sorted the resulting $n^2$ values in non-decreasing order. You need to find the $k$-th of them.</p><p>The definition of <span class="tex-font-style-tt">xor</span> is as follows.</p><p>Given two integers $x$ and $y$, consider their binary representations (possibly with leading zeros): $x_k \dots x_2 x_1 x_0$ and $y_k \dots y_2 y_1 y_0$ (where $k$ is any number so that all bits of $x$ and $y$ can be represented). Here, $x_i$ is the $i$-th bit of the number $x$ and $y_i$ is the $i$-th bit of the number $y$. Let $r = x \oplus y$ be the result of the <span class="tex-font-style-tt">xor</span> operation of $x$ and $y$. Then $r$ is defined as $r_k \dots r_2 r_1 r_0$ where:</p><p>$$ r_i = \left\{ \begin{aligned} 1, ~ \text{if} ~ x_i \ne y_i \\ 0, ~ \text{if} ~ x_i = y_i \end{aligned} \right. $$</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le n \le 10^6$, $1 \le k \le n^2$)&nbsp;— the number of vertices in the tree and the number of path in the list with non-decreasing order.</p><p>Each of the following $n - 1$ lines contains two integers $p_i$ and $w_i$ ($1 \le p_i \le i$, $0 \le w_i &lt; 2^{62}$)&nbsp;— the ancestor of vertex $i + 1$ and the weight of the corresponding edge.</p></div><div class="output-specification"><p>Print one integer: $k$-th smallest xor of a path in the tree.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le n \le 10^6$, $1 \le k \le n^2$)&nbsp;— the number of vertices in the tree and the number of path in the list with non-decreasing order.</p><p>Each of the following $n - 1$ lines contains two integers $p_i$ and $w_i$ ($1 \le p_i \le i$, $0 \le w_i &lt; 2^{62}$)&nbsp;— the ancestor of vertex $i + 1$ and the weight of the corresponding edge.</p>

## Output

<p>Print one integer: $k$-th smallest xor of a path in the tree.</p>





```input1
2 1
1 3

```




```input2
3 6
1 2
1 3

```




```output1
0

```




```output2
2

```



## Note

<p>The tree in the second sample test looks like this:</p><p><img class="tex-graphics" src="file://sJTxab5u.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>For such a tree in total $9$ paths exist: </p><ol> <li> $1 \to 1$ of value $0$ </li><li> $2 \to 2$ of value $0$ </li><li> $3 \to 3$ of value $0$ </li><li> $2 \to 3$ (goes through $1$) of value $1 = 2 \oplus 3$ </li><li> $3 \to 2$ (goes through $1$) of value $1 = 2 \oplus 3$ </li><li> $1 \to 2$ of value $2$ </li><li> $2 \to 1$ of value $2$ </li><li> $1 \to 3$ of value $3$ </li><li> $3 \to 1$ of value $3$ </li></ol>
