## Description

<div><p>You are given a rooted tree on $n$ vertices, its root is the vertex number $1$. The $i$-th vertex contains a number $w_i$. Split it into the minimum possible number of vertical paths in such a way that each path contains no more than $L$ vertices and the sum of integers $w_i$ on each path does not exceed $S$. Each vertex should belong to exactly one path.</p><p>A vertical path is a sequence of vertices $v_1, v_2, \ldots, v_k$ where $v_i$ ($i \ge 2$) is the parent of $v_{i - 1}$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $L$, $S$ ($1 \le n \le 10^5$, $1 \le L \le 10^5$, $1 \le S \le 10^{18}$)&nbsp;— the number of vertices, the maximum number of vertices in one path and the maximum sum in one path.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($1 \le w_i \le 10^9$)&nbsp;— the numbers in the vertices of the tree.</p><p>The third line contains $n - 1$ integers $p_2, \ldots, p_n$ ($1 \le p_i &lt; i$), where $p_i$ is the parent of the $i$-th vertex in the tree.</p></div><div class="output-specification"><p>Output one number &nbsp;— the minimum number of vertical paths. If it is impossible to split the tree, output $-1$.</p></div>

## Input

<p>The first line contains three integers $n$, $L$, $S$ ($1 \le n \le 10^5$, $1 \le L \le 10^5$, $1 \le S \le 10^{18}$)&nbsp;— the number of vertices, the maximum number of vertices in one path and the maximum sum in one path.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($1 \le w_i \le 10^9$)&nbsp;— the numbers in the vertices of the tree.</p><p>The third line contains $n - 1$ integers $p_2, \ldots, p_n$ ($1 \le p_i &lt; i$), where $p_i$ is the parent of the $i$-th vertex in the tree.</p>

## Output

<p>Output one number &nbsp;— the minimum number of vertical paths. If it is impossible to split the tree, output $-1$.</p>





```input1
3 1 3
1 2 3
1 1

```




```input2
3 3 6
1 2 3
1 1

```




```input3
1 1 10000
10001

```




```output1
3
```




```output2
2
```




```output3
-1
```



## Note

<p>In the first sample the tree is split into $\{1\},\ \{2\},\ \{3\}$.</p><p>In the second sample the tree is split into $\{1,\ 2\},\ \{3\}$ or $\{1,\ 3\},\ \{2\}$.</p><p>In the third sample it is impossible to split the tree.</p>
