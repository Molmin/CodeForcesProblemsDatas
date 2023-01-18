## Description

<div><p>As the name of the task implies, you are asked to do some work with segments and trees.</p><p>Recall that a tree is a connected undirected graph such that there is exactly one simple path between every pair of its vertices.</p><p>You are given $n$ segments $[l_1, r_1], [l_2, r_2], \dots, [l_n, r_n]$, $l_i &lt; r_i$ for every $i$. It is guaranteed that all segments' endpoints are integers, and all endpoints are unique — there is no pair of segments such that they start in the same point, end in the same point or one starts in the same point the other one ends.</p><p>Let's generate a graph with $n$ vertices from these segments. Vertices $v$ and $u$ are connected by an edge if and only if segments $[l_v, r_v]$ and $[l_u, r_u]$ intersect and neither of it lies fully inside the other one.</p><p>For example, pairs $([1, 3], [2, 4])$ and $([5, 10], [3, 7])$ will induce the edges but pairs $([1, 2], [3, 4])$ and $([5, 7], [3, 10])$ will not.</p><p>Determine if the resulting graph is a tree or not.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of segments.</p><p>The $i$-th of the next $n$ lines contain the description of the $i$-th segment — two integers $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 2n$).</p><p>It is guaranteed that all segments borders are pairwise distinct. </p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if the resulting graph is a tree and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of segments.</p><p>The $i$-th of the next $n$ lines contain the description of the $i$-th segment — two integers $l_i$ and $r_i$ ($1 \le l_i &lt; r_i \le 2n$).</p><p>It is guaranteed that all segments borders are pairwise distinct. </p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if the resulting graph is a tree and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
6
9 12
2 11
1 3
6 10
5 7
4 8
```




```input2
5
1 3
2 4
5 9
6 8
7 10
```




```input3
5
5 8
3 6
2 9
7 10
1 4
```




```output1
YES
```




```output2
NO
```




```output3
NO
```



## Note

<p>The graph corresponding to the first example:</p><p><img class="tex-graphics" src="file://grI8zGCp.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The graph corresponding to the second example:</p><p><img class="tex-graphics" src="file://R3HteJyp.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The graph corresponding to the third example:</p><p><img class="tex-graphics" src="file://bGiIKSss.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
