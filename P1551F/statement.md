## Description

<div><p>A tree is an undirected connected graph without cycles.</p><p>You are given a tree of $n$ vertices. Find the number of ways to choose exactly $k$ vertices in this tree (i. e. a $k$-element subset of vertices) so that all pairwise distances between the selected vertices are equal (in other words, there exists an integer $c$ such that for all $u, v$ ($u \ne v$, $u, v$ are in selected vertices) $d_{u,v}=c$, where $d_{u,v}$ is the distance from $u$ to $v$).</p><p>Since the answer may be very large, you need to output it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case is preceded by an empty line.</p><p>Each test case consists of several lines. The first line of the test case contains two integers $n$ and $k$ ($2 \le k \le n \le 100$) — the number of vertices in the tree and the number of vertices to be selected, respectively. Then $n - 1$ lines follow, each of them contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) which describe a pair of vertices connected by an edge. It is guaranteed that the given graph is a tree and has no loops or multiple edges.</p></div><div class="output-specification"><p>For each test case output in a separate line a single integer — the number of ways to select exactly $k$ vertices so that for all pairs of selected vertices the distances between the vertices in the pairs are equal, modulo $10^9 + 7$ (in other words, print the remainder when divided by $1000000007$).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case is preceded by an empty line.</p><p>Each test case consists of several lines. The first line of the test case contains two integers $n$ and $k$ ($2 \le k \le n \le 100$) — the number of vertices in the tree and the number of vertices to be selected, respectively. Then $n - 1$ lines follow, each of them contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \neq v$) which describe a pair of vertices connected by an edge. It is guaranteed that the given graph is a tree and has no loops or multiple edges.</p>

## Output

<p>For each test case output in a separate line a single integer — the number of ways to select exactly $k$ vertices so that for all pairs of selected vertices the distances between the vertices in the pairs are equal, modulo $10^9 + 7$ (in other words, print the remainder when divided by $1000000007$).</p>





```input1
3

4 2
1 2
2 3
2 4

3 3
1 2
2 3

5 3
1 2
2 3
2 4
4 5
```




```output1
6
0
1
```


