## Description

<div><p>You are given a tree with $n$ vertices. Each vertex $i$ has a value $a_i$ associated with it.</p><p>Let us root the tree at some vertex $v$. The vertex $v$ is called a <span class="tex-font-style-it">distinctive root</span> if the following holds: in all paths that start at $v$ and end at some other node, all the values encountered are distinct. Two different paths may have values in common but a single path must have all distinct values.</p><p>Find the number of <span class="tex-font-style-it">distinctive roots</span> in the tree.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1 \le n \le 2\cdot10^5$) — the number of vertices in the tree.</p><p>The next line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>The following $n-1$ lines each contain two space-separated integers $u$ and $v$ ($1 \le u$, $v \le n$), denoting an edge from $u$ to $v$.</p><p>It is guaranteed that the edges form a tree.</p></div><div class="output-specification"><p>Print a single integer — the number of <span class="tex-font-style-it">distinctive roots</span> in the tree.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1 \le n \le 2\cdot10^5$) — the number of vertices in the tree.</p><p>The next line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>The following $n-1$ lines each contain two space-separated integers $u$ and $v$ ($1 \le u$, $v \le n$), denoting an edge from $u$ to $v$.</p><p>It is guaranteed that the edges form a tree.</p>

## Output

<p>Print a single integer — the number of <span class="tex-font-style-it">distinctive roots</span> in the tree.</p>





```input1
5
2 5 1 1 4
1 2
1 3
2 4
2 5
```




```input2
5
2 1 1 1 4
1 2
1 3
2 4
2 5
```




```output1
3
```




```output2
0
```



## Note

<p>In the first example, $1$, $2$ and $5$ are <span class="tex-font-style-it">distinctive roots</span>.</p>
