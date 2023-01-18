## Description

<div><p>Ramesses knows a lot about problems involving trees (undirected connected graphs without cycles)!</p><p>He created a new useful tree decomposition, but he does not know how to construct it, so he asked you for help!</p><p>The decomposition is the splitting the edges of the tree in some simple paths in such a way that each two paths have at least one common vertex. Each edge of the tree should be in exactly one path.</p><p>Help Remesses, find such a decomposition of the tree or derermine that there is no such decomposition.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 10^{5}$) the number of nodes in the tree.</p><p>Each of the next $n - 1$ lines contains two integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$)&nbsp;— the edges of the tree. It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>If there are no decompositions, print the only line containing "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">Yes</span>", and in the second line print the number of paths in the decomposition $m$. </p><p>Each of the next $m$ lines should contain two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n$, $u_i \neq v_i$) denoting that one of the paths in the decomposition is the simple path between nodes $u_i$ and $v_i$. </p><p>Each pair of paths in the decomposition should have at least one common vertex, and each edge of the tree should be presented in exactly one path. You can print the paths and the ends of each path in arbitrary order.</p><p>If there are multiple decompositions, print any.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 10^{5}$) the number of nodes in the tree.</p><p>Each of the next $n - 1$ lines contains two integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$)&nbsp;— the edges of the tree. It is guaranteed that the given edges form a tree.</p>

## Output

<p>If there are no decompositions, print the only line containing "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">Yes</span>", and in the second line print the number of paths in the decomposition $m$. </p><p>Each of the next $m$ lines should contain two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n$, $u_i \neq v_i$) denoting that one of the paths in the decomposition is the simple path between nodes $u_i$ and $v_i$. </p><p>Each pair of paths in the decomposition should have at least one common vertex, and each edge of the tree should be presented in exactly one path. You can print the paths and the ends of each path in arbitrary order.</p><p>If there are multiple decompositions, print any.</p>





```input1
4
1 2
2 3
3 4

```




```input2
6
1 2
2 3
3 4
2 5
3 6

```




```input3
5
1 2
1 3
1 4
1 5

```




```output1
Yes
1
1 4

```




```output2
No

```




```output3
Yes
4
1 2
1 3
1 4
1 5

```



## Note

<p>The tree from the first example is shown on the picture below: <img class="tex-graphics" src="file://lDptQy7W.png" style="max-width: 100.0%;max-height: 100.0%;"> The number next to each edge corresponds to the path number in the decomposition. It is easy to see that this decomposition suits the required conditions.</p><p>The tree from the second example is shown on the picture below: <img class="tex-graphics" src="file://SwarjXpx.png" style="max-width: 100.0%;max-height: 100.0%;"> We can show that there are no valid decompositions of this tree.</p><p>The tree from the third example is shown on the picture below: <img class="tex-graphics" src="file://iME0G4SH.png" style="max-width: 100.0%;max-height: 100.0%;"> The number next to each edge corresponds to the path number in the decomposition. It is easy to see that this decomposition suits the required conditions.</p>
