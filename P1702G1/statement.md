## Description

<div><p><span class="tex-font-style-bf">This is an easy version of the problem. The only difference between an easy and a hard version is in the number of queries.</span></p><p>Polycarp grew a tree from $n$ vertices. We remind you that a tree of $n$ vertices is an undirected connected graph of $n$ vertices and $n-1$ edges that does not contain cycles.</p><p>He calls a set of vertices <span class="tex-font-style-it">passable</span> if there is such a path in the tree that passes through each vertex of this set without passing through any edge twice. The path can visit other vertices (not from this set).</p><p>In other words, a set of vertices is called <span class="tex-font-style-it">passable</span> if there is a simple path that passes through all the vertices of this set (and possibly some other).</p><p>For example, for a tree below sets $\{3, 2, 5\}$, $\{1, 5, 4\}$, $\{1, 4\}$ are <span class="tex-font-style-it">passable</span>, and $\{1, 3, 5\}$, $\{1, 2, 3, 4, 5\}$ are not.</p><center> <img class="tex-graphics" src="file://YGsi7xeW.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center><p>Polycarp asks you to answer $q$ queries. Each query is a set of vertices. For each query, you need to determine whether the corresponding set of vertices is <span class="tex-font-style-bf">passable</span>.</p></div><div class="input-specification"><p>The first line of input contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — number of vertices.</p><p>Following $n - 1$ lines a description of the tree..</p><p>Each line contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \ne v$) — indices of vertices connected by an edge.</p><p>Following line contains single integer $q$ ($1 \le q \le 5$)&nbsp;— number of queries.</p><p>The following $2 \cdot q$ lines contain descriptions of sets.</p><p>The first line of the description contains an integer $k$ ($1 \le k \le n$) — the size of the set.</p><p>The second line of the description contains $k$ of distinct integers $p_1, p_2, \dots, p_k$ ($1 \le p_i \le n$) — indices of the vertices of the set.</p><p>It is guaranteed that the sum of $k$ values for all queries does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output $q$ lines, each of which contains the answer to the corresponding query. As an answer, output "<span class="tex-font-style-tt">YES</span>" if the set is <span class="tex-font-style-bf">passable</span>, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line of input contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — number of vertices.</p><p>Following $n - 1$ lines a description of the tree..</p><p>Each line contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \ne v$) — indices of vertices connected by an edge.</p><p>Following line contains single integer $q$ ($1 \le q \le 5$)&nbsp;— number of queries.</p><p>The following $2 \cdot q$ lines contain descriptions of sets.</p><p>The first line of the description contains an integer $k$ ($1 \le k \le n$) — the size of the set.</p><p>The second line of the description contains $k$ of distinct integers $p_1, p_2, \dots, p_k$ ($1 \le p_i \le n$) — indices of the vertices of the set.</p><p>It is guaranteed that the sum of $k$ values for all queries does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output $q$ lines, each of which contains the answer to the corresponding query. As an answer, output "<span class="tex-font-style-tt">YES</span>" if the set is <span class="tex-font-style-bf">passable</span>, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1
5
1 2
2 3
2 4
4 5
5
3
3 2 5
5
1 2 3 4 5
2
1 4
3
1 3 5
3
1 5 4
```




```input2
5
1 2
3 2
2 4
5 2
4
2
3 1
3
3 4 5
3
2 3 5
1
1
```




```output1
YES
NO
YES
NO
YES
```




```output2
YES
NO
YES
YES
```


