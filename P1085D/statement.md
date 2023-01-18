## Description

<div><p>You are given a tree (an undirected connected graph without cycles) and an integer $s$.</p><p>Vanya wants to put weights on all edges of the tree so that all weights are non-negative real numbers and their sum is $s$. At the same time, he wants to make the diameter of the tree as small as possible.</p><p>Let's define the diameter of a weighed tree as the maximum sum of the weights of the edges lying on the path between two some vertices of the tree. In other words, the diameter of a weighed tree is the length of the longest simple path in the tree, where length of a path is equal to the sum of weights over all edges in the path.</p><p>Find the minimum possible diameter that Vanya can get.</p></div><div class="input-specification"><p>The first line contains two integer numbers $n$ and $s$ ($2 \leq n \leq 10^5$, $1 \leq s \leq 10^9$) — the number of vertices in the tree and the sum of edge weights.</p><p>Each of the following $n−1$ lines contains two space-separated integer numbers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$) — the indexes of vertices connected by an edge. The edges are undirected.</p><p>It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>Print the minimum diameter of the tree that Vanya can get by placing some non-negative real weights on its edges with the sum equal to $s$.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is considered correct if $\frac {|a-b|} {max(1, b)} \leq 10^{-6}$.</p></div>

## Input

<p>The first line contains two integer numbers $n$ and $s$ ($2 \leq n \leq 10^5$, $1 \leq s \leq 10^9$) — the number of vertices in the tree and the sum of edge weights.</p><p>Each of the following $n−1$ lines contains two space-separated integer numbers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$) — the indexes of vertices connected by an edge. The edges are undirected.</p><p>It is guaranteed that the given edges form a tree.</p>

## Output

<p>Print the minimum diameter of the tree that Vanya can get by placing some non-negative real weights on its edges with the sum equal to $s$.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is considered correct if $\frac {|a-b|} {max(1, b)} \leq 10^{-6}$.</p>





```input1
4 3
1 2
1 3
1 4
```




```input2
6 1
2 1
2 3
2 5
5 4
5 6
```




```input3
5 5
1 2
2 3
3 4
3 5
```




```output1
2.000000000000000000
```




```output2
0.500000000000000000
```




```output3
3.333333333333333333
```



## Note

<p>In the first example it is necessary to put weights like this:</p><center> <img class="tex-graphics" src="file://MtY0E62f.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It is easy to see that the diameter of this tree is $2$. It can be proved that it is the minimum possible diameter.</p><p>In the second example it is necessary to put weights like this:</p><center> <img class="tex-graphics" src="file://RJ3hdsbp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
