## Description

<div><p>// <span class="tex-font-style-it">We decided to drop the legend about the power sockets but feel free to come up with your own :^)</span></p><p>Define a chain: </p><ul> <li> a chain of length $1$ is a single vertex; </li><li> a chain of length $x$ is a chain of length $x-1$ with a new vertex connected to the end of it with a single edge. </li></ul><p>You are given $n$ chains of lengths $l_1, l_2, \dots, l_n$. You plan to build a tree using some of them.</p><ul> <li> Each vertex of the tree is either white or black. </li><li> The tree initially only has a white root vertex. </li><li> All chains initially consist only of white vertices. </li><li> You can take one of the chains and connect any of its vertices to any white vertex of the tree with an edge. The chain becomes part of the tree. Both endpoints of this edge become black. </li><li> Each chain can be used no more than once. </li><li> Some chains can be left unused. </li></ul><p>The distance between two vertices of the tree is the number of edges on the shortest path between them.</p><p>If there is at least $k$ white vertices in the resulting tree, then the value of the tree is the distance between the root and the $k$-th closest white vertex.</p><p>What's the minimum value of the tree you can obtain? If there is no way to build a tree with at least $k$ white vertices, then print <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $2 \le k \le 10^9$)&nbsp;— the number of chains and the minimum number of white vertices a tree should have to have a value.</p><p>The second line contains $n$ integers $l_1, l_2, \dots, l_n$ ($3 \le l_i \le 2 \cdot 10^5$)&nbsp;— the lengths of the chains.</p></div><div class="output-specification"><p>Print a single integer. If there is no way to build a tree with at least $k$ white vertices, then print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum value the tree can have.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $2 \le k \le 10^9$)&nbsp;— the number of chains and the minimum number of white vertices a tree should have to have a value.</p><p>The second line contains $n$ integers $l_1, l_2, \dots, l_n$ ($3 \le l_i \le 2 \cdot 10^5$)&nbsp;— the lengths of the chains.</p>

## Output

<p>Print a single integer. If there is no way to build a tree with at least $k$ white vertices, then print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum value the tree can have.</p>





```input1
1 2
3
```




```input2
3 3
4 3 3
```




```input3
3 5
4 3 4
```




```input4
2 10
5 7
```




```output1
2
```




```output2
3
```




```output3
4
```




```output4
-1
```



## Note

<center> <img class="tex-graphics" src="file://MUd1wAmW.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>You are allowed to not use all the chains, so it's optimal to only use chain of length $4$ in the second example.</p>
