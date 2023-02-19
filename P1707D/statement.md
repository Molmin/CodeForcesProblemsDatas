## Description

<div><p>Kawashiro Nitori is a girl who loves competitive programming. One day she found a rooted tree consisting of $n$ vertices. The root is vertex $1$. As an advanced problem setter, she quickly thought of a problem.</p><p>Kawashiro Nitori has a vertex set $U=\{1,2,\ldots,n\}$. She's going to play a game with the tree and the set. In each operation, she will choose a vertex set $T$, where $T$ is a <span class="tex-font-style-it">partial virtual tree</span> of $U$, and change $U$ into $T$.</p><p>A vertex set $S_1$ is a partial virtual tree of a vertex set $S_2$, if $S_1$ is a subset of $S_2$, $S_1 \neq S_2$, and for all pairs of vertices $i$ and $j$ in $S_1$, $\operatorname{LCA}(i,j)$ is in $S_1$, where $\operatorname{LCA}(x,y)$ denotes the <a href="https://en.wikipedia.org/wiki/Lowest_common_ancestor">lowest common ancestor</a> of vertices $x$ and $y$ on the tree. Note that a vertex set can have many different partial virtual trees.</p><p>Kawashiro Nitori wants to know for each possible $k$, if she performs the operation <span class="tex-font-style-bf">exactly</span> $k$ times, in how many ways she can make $U=\{1\}$ in the end? Two ways are considered different if there exists an integer $z$ ($1 \le z \le k$) such that after $z$ operations the sets $U$ are different.</p><p>Since the answer could be very large, you need to find it modulo $p$. It's guaranteed that $p$ is a prime number.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $p$ ($2 \le n \le 2000$, $10^8 + 7 \le p \le 10^9+9$). It's guaranteed that $p$ is a prime number.</p><p>Each of the next $n-1$ lines contains two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n$), representing an edge between $u_i$ and $v_i$.</p><p>It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>The only line contains $n-1$ integers&nbsp;— the answer modulo $p$ for $k=1,2,\ldots,n-1$.</p></div>

## Input

<p>The first line contains two integers $n$ and $p$ ($2 \le n \le 2000$, $10^8 + 7 \le p \le 10^9+9$). It's guaranteed that $p$ is a prime number.</p><p>Each of the next $n-1$ lines contains two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n$), representing an edge between $u_i$ and $v_i$.</p><p>It is guaranteed that the given edges form a tree.</p>

## Output

<p>The only line contains $n-1$ integers&nbsp;— the answer modulo $p$ for $k=1,2,\ldots,n-1$.</p>





```input1
4 998244353
1 2
2 3
1 4
```




```input2
7 100000007
1 2
1 3
2 4
2 5
3 6
3 7
```




```input3
8 1000000007
1 2
2 3
3 4
4 5
5 6
6 7
7 8
```




```output1
1 6 6
```




```output2
1 47 340 854 880 320
```




```output3
1 126 1806 8400 16800 15120 5040
```



## Note

<p>In the first test case, when $k=1$, the only possible way is:</p><ol> <li> $\{1,2,3,4\} \to \{1\}$. </li></ol><p>When $k=2$, there are $6$ possible ways:</p><ol> <li> $\{1,2,3,4\} \to \{1,2\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,2,3\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,2,4\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,3\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,3,4\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,4\} \to \{1\}$. </li></ol><p>When $k=3$, there are $6$ possible ways:</p><ol> <li> $\{1,2,3,4\} \to \{1,2,3\} \to \{1,2\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,2,3\} \to \{1,3\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,2,4\} \to \{1,2\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,2,4\} \to \{1,4\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,3,4\} \to \{1,3\} \to \{1\}$; </li><li> $\{1,2,3,4\} \to \{1,3,4\} \to \{1,4\} \to \{1\}$. </li></ol>
