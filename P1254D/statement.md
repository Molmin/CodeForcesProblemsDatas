## Description

<div><p>Hanh is a famous biologist. He loves growing trees and doing experiments on his own garden.</p><p>One day, he got a tree consisting of $n$ vertices. Vertices are numbered from $1$ to $n$. A tree with $n$ vertices is an undirected connected graph with $n-1$ edges. Initially, Hanh sets the value of every vertex to $0$.</p><p>Now, Hanh performs $q$ operations, each is either of the following types: </p><ul> <li> Type $1$: Hanh selects a vertex $v$ and an integer $d$. Then he chooses some vertex $r$ <span class="tex-font-style-bf">uniformly at random</span>, lists all vertices $u$ such that the path from $r$ to $u$ passes through $v$. Hanh then increases the value of all such vertices $u$ by $d$. </li><li> Type $2$: Hanh selects a vertex $v$ and calculates the expected value of $v$. </li></ul><p>Since Hanh is good at biology but not math, he needs your help on these operations.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \leq n, q \leq 150\,000$)&nbsp;— the number of vertices on Hanh's tree and the number of operations he performs.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n$), denoting that there is an edge connecting two vertices $u$ and $v$. It is guaranteed that these $n - 1$ edges form a tree.</p><p>Each of the last $q$ lines describes an operation in either formats: </p><ul> <li> $1$ $v$ $d$ ($1 \leq v \leq n, 0 \leq d \leq 10^7$), representing a first-type operation. </li><li> $2$ $v$ ($1 \leq v \leq n$), representing a second-type operation. </li></ul><p>It is guaranteed that there is at least one query of the second type.</p></div><div class="output-specification"><p>For each operation of the second type, write the expected value on a single line. </p><p>Let $M = 998244353$, it can be shown that the expected value can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \leq n, q \leq 150\,000$)&nbsp;— the number of vertices on Hanh's tree and the number of operations he performs.</p><p>Each of the next $n - 1$ lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n$), denoting that there is an edge connecting two vertices $u$ and $v$. It is guaranteed that these $n - 1$ edges form a tree.</p><p>Each of the last $q$ lines describes an operation in either formats: </p><ul> <li> $1$ $v$ $d$ ($1 \leq v \leq n, 0 \leq d \leq 10^7$), representing a first-type operation. </li><li> $2$ $v$ ($1 \leq v \leq n$), representing a second-type operation. </li></ul><p>It is guaranteed that there is at least one query of the second type.</p>

## Output

<p>For each operation of the second type, write the expected value on a single line. </p><p>Let $M = 998244353$, it can be shown that the expected value can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p>





```input1
5 12
1 2
1 3
2 4
2 5
1 1 1
2 1
2 2
2 3
2 4
2 5
1 2 2
2 1
2 2
2 3
2 4
2 5
```




```output1
1
199648871
399297742
199648871
199648871
598946614
199648873
2
2
2
```



## Note

<p>The image below shows the tree in the example:</p><center> <img class="tex-graphics" height="265px" src="file://qbMUd9KE.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> </center><p>For the first query, where $v = 1$ and $d = 1$: </p><ul> <li> If $r = 1$, the values of all vertices get increased. </li><li> If $r = 2$, the values of vertices $1$ and $3$ get increased. </li><li> If $r = 3$, the values of vertices $1$, $2$, $4$ and $5$ get increased. </li><li> If $r = 4$, the values of vertices $1$ and $3$ get increased. </li><li> If $r = 5$, the values of vertices $1$ and $3$ get increased. </li></ul><p>Hence, the expected values of all vertices after this query are ($1, 0.4, 0.8, 0.4, 0.4$).</p><p>For the second query, where $v = 2$ and $d = 2$: </p><ul> <li> If $r = 1$, the values of vertices $2$, $4$ and $5$ get increased. </li><li> If $r = 2$, the values of all vertices get increased. </li><li> If $r = 3$, the values of vertices $2$, $4$ and $5$ get increased. </li><li> If $r = 4$, the values of vertices $1$, $2$, $3$ and $5$ get increased. </li><li> If $r = 5$, the values of vertices $1$, $2$, $3$ and $4$ get increased. </li></ul><p>Hence, the expected values of all vertices after this query are ($2.2, 2.4, 2, 2, 2$).</p>
