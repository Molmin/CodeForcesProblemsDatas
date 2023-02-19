## Description

<div><p>You are given a tree with $n$ vertices numbered from $1$ to $n$. The height of the $i$-th vertex is $h_i$. You can place any number of towers into vertices, for each tower you can choose which vertex to put it in, as well as choose its efficiency. Setting up a tower with efficiency $e$ costs $e$ coins, where $e &gt; 0$.</p><p>It is considered that a vertex $x$ gets a signal if for some pair of towers at the vertices $u$ and $v$ ($u \neq v$, but it is allowed that $x = u$ or $x = v$) with efficiencies $e_u$ and $e_v$, respectively, it is satisfied that $\min(e_u, e_v) \geq h_x$ and $x$ lies on the path between $u$ and $v$.</p><p>Find the minimum number of coins required to set up towers so that you can get a signal at all vertices.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \le n \le 200\,000$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $h_i$ ($1 \le h_i \le 10^9$)&nbsp;— the heights of the vertices.</p><p>Each of the next $n - 1$ lines contain a pair of numbers $v_i, u_i$ ($1 \le v_i, u_i \le n$)&nbsp;— an edge of the tree. It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum required number of coins.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \le n \le 200\,000$)&nbsp;— the number of vertices in the tree.</p><p>The second line contains $n$ integers $h_i$ ($1 \le h_i \le 10^9$)&nbsp;— the heights of the vertices.</p><p>Each of the next $n - 1$ lines contain a pair of numbers $v_i, u_i$ ($1 \le v_i, u_i \le n$)&nbsp;— an edge of the tree. It is guaranteed that the given edges form a tree.</p>

## Output

<p>Print one integer&nbsp;— the minimum required number of coins.</p>





```input1
3
1 2 1
1 2
2 3
```




```input2
5
1 3 3 1 3
1 3
5 4
4 3
2 3
```




```input3
2
6 1
1 2
```




```output1
4
```




```output2
7
```




```output3
12
```



## Note

<p>In the first test case it's optimal to install two towers with efficiencies $2$ at vertices $1$ and $3$.</p><p>In the second test case it's optimal to install a tower with efficiency $1$ at vertex $1$ and two towers with efficiencies $3$ at vertices $2$ and $5$.</p><p>In the third test case it's optimal to install two towers with efficiencies $6$ at vertices $1$ and $2$.</p>
