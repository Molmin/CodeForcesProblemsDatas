## Description

<div><p>Let's call a graph with $n$ vertices, each of which has it's own point $A_i = (x_i, y_i)$ with integer coordinates, a <span class="tex-font-style-it">planar tree</span> if:</p><ul> <li> All points $A_1, A_2, \ldots, A_n$ are different and no three points lie on the same line. </li><li> The graph is a tree, i.e. there are exactly $n-1$ edges there exists a path between any pair of vertices. </li><li> For all pairs of edges $(s_1, f_1)$ and $(s_2, f_2)$, such that $s_1 \neq s_2, s_1 \neq f_2,$ $f_1 \neq s_2$, and $f_1 \neq f_2$, the segments $A_{s_1} A_{f_1}$ and $A_{s_2} A_{f_2}$ don't intersect. </li></ul><p>Imagine a planar tree with $n$ vertices. Consider the convex hull of points $A_1, A_2, \ldots, A_n$. Let's call this tree a <span class="tex-font-style-it">spiderweb tree</span> if for all $1 \leq i \leq n$ the following statements are true:</p><ul> <li> All leaves (vertices with degree $\leq 1$) of the tree lie on the border of the convex hull. </li><li> All vertices on the border of the convex hull are leaves. </li></ul><p>An example of a spiderweb tree: </p><center> <img class="tex-graphics" src="file://2AQezGz6.png" style="max-width: 100.0%;max-height: 100.0%;">   </center><p>The points $A_3, A_6, A_7, A_4$ lie on the convex hull and the leaf vertices of the tree are $3, 6, 7, 4$.</p><p>Refer to the notes for more examples.</p><p>Let's call the subset $S \subset \{1, 2, \ldots, n\}$ of vertices a <span class="tex-font-style-it">subtree</span> of the tree if for all pairs of vertices in $S$, there exists a path that contains only vertices from $S$. Note that any subtree of the planar tree is a planar tree.</p><p>You are given a planar tree with $n$ vertexes. Let's call a partition of the set $\{1, 2, \ldots, n\}$ into non-empty subsets $A_1, A_2, \ldots, A_k$ (i.e. $A_i \cap A_j = \emptyset$ for all $1 \leq i &lt; j \leq k$ and $A_1 \cup A_2 \cup \ldots \cup A_k = \{1, 2, \ldots, n\}$) good if for all $1 \leq i \leq k$, the subtree $A_i$ is a spiderweb tree. Two partitions are different if there exists some set that lies in one parition, but not the other.</p><p>Find the number of good partitions. Since this number can be very large, find it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of vertices in the tree.</p><p>The next $n$ lines each contain two integers $x_i, y_i$ ($-10^9 \leq x_i, y_i \leq 10^9$) &nbsp;— the coordinates of $i$-th vertex, $A_i$.</p><p>The next $n-1$ lines contain two integers $s, f$ ($1 \leq s, f \leq n$)&nbsp;— the edges $(s, f)$ of the tree.</p><p>It is guaranteed that all given points are different and that no three of them lie at the same line. Additionally, it is guaranteed that the given edges and coordinates of the points describe a planar tree.</p></div><div class="output-specification"><p>Print one integer &nbsp;— the number of good partitions of vertices of the given planar tree, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of vertices in the tree.</p><p>The next $n$ lines each contain two integers $x_i, y_i$ ($-10^9 \leq x_i, y_i \leq 10^9$) &nbsp;— the coordinates of $i$-th vertex, $A_i$.</p><p>The next $n-1$ lines contain two integers $s, f$ ($1 \leq s, f \leq n$)&nbsp;— the edges $(s, f)$ of the tree.</p><p>It is guaranteed that all given points are different and that no three of them lie at the same line. Additionally, it is guaranteed that the given edges and coordinates of the points describe a planar tree.</p>

## Output

<p>Print one integer &nbsp;— the number of good partitions of vertices of the given planar tree, modulo $998\,244\,353$.</p>





```input1
4
0 0
0 1
-1 -1
1 -1
1 2
1 3
1 4
```




```input2
5
3 2
0 -3
-5 -3
5 -5
4 5
4 2
4 1
5 2
2 3
```




```input3
6
4 -5
0 1
-2 8
3 -10
0 -1
-4 -5
2 5
3 2
1 2
4 6
4 2
```




```input4
8
0 0
-1 2
-2 5
-5 1
1 3
0 3
2 4
-1 -4
1 2
3 2
5 6
4 2
1 5
5 7
5 8
```




```output1
5
```




```output2
8
```




```output3
13
```




```output4
36
```



## Note

<center> <img class="tex-graphics" src="file://p0DE0htf.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture for the first sample.</span> </center><p>In the first test case, all good partitions are:</p><ol> <li> $\{1\}$, $\{2\}$, $\{3\}$, $\{4\}$; </li><li> $\{1, 2\}$, $\{3\}$, $\{4\}$; </li><li> $\{1, 3\}$, $\{2\}$, $\{4\}$; </li><li> $\{1, 4\}$, $\{2\}$, $\{3\}$; </li><li> $\{1, 2, 3, 4\}$. </li></ol><p>The partition $\{1, 2, 3\}$, $\{4\}$ isn't good, because the subtree $\{1, 2, 3\}$ isn't spiderweb tree, since the non-leaf vertex $1$ lies on the convex hull.</p><p>The partition $\{2, 3, 4\}$, $\{1\}$ isn't good, because the subset $\{2, 3, 4\}$ isn't a subtree.</p><center> <img class="tex-graphics" src="file://IGoImQfW.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture for the second sample.</span> </center><p>In the second test case, the given tree isn't a spiderweb tree, because the leaf vertex $1$ doesn't lie on the convex hull. However, the subtree $\{2, 3, 4, 5\}$ is a spiderweb tree.</p><center> <img class="tex-graphics" src="file://Xlcru4hH.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture for the third sample.</span> </center><center> <img class="tex-graphics" src="file://ZW9eO8EI.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The picture for the fourth sample.</span> </center><p>In the fourth test case, the partition $\{1, 2, 3, 4\}$, $\{5, 6, 7, 8\}$ is good because all subsets are spiderweb subtrees.</p>
