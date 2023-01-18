## Description

<div><p>You're given a tree consisting of $n$ nodes. Every node $u$ has a weight $a_u$. You want to choose an integer $k$ $(1 \le k \le n)$ and then choose $k$ connected components of nodes that don't overlap (i.e every node is in at most 1 component). Let the set of nodes you chose be $s$. You want to maximize:</p><p>$$\frac{\sum\limits_{u \in s} a_u}{k}$$</p><p>In other words, you want to maximize the sum of weights of nodes in $s$ divided by the number of connected components you chose. Also, if there are several solutions, you want to <span class="tex-font-style-bf">maximize $k$</span>.</p><p>Note that adjacent nodes <span class="tex-font-style-bf">can</span> belong to different components. Refer to the third sample.</p></div><div class="input-specification"><p>The first line contains the integer $n$ $(1 \le n \le 3 \cdot 10^5)$, the number of nodes in the tree.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\dots$, $a_n$ $(|a_i| \le 10^9)$, the weights of the nodes.</p><p>The next $n-1$ lines, each contains 2 space-separated integers $u$ and $v$ $(1 \le u,v \le n)$ which means there's an edge between $u$ and $v$.</p></div><div class="output-specification"><p>Print the answer as a <span class="tex-font-style-bf">non-reduced</span> fraction represented by 2 space-separated integers. The fraction itself should be maximized and if there are several possible ways, you should maximize the denominator. See the samples for a better understanding.</p></div>

## Input

<p>The first line contains the integer $n$ $(1 \le n \le 3 \cdot 10^5)$, the number of nodes in the tree.</p><p>The second line contains $n$ space-separated integers $a_1$, $a_2$, $\dots$, $a_n$ $(|a_i| \le 10^9)$, the weights of the nodes.</p><p>The next $n-1$ lines, each contains 2 space-separated integers $u$ and $v$ $(1 \le u,v \le n)$ which means there's an edge between $u$ and $v$.</p>

## Output

<p>Print the answer as a <span class="tex-font-style-bf">non-reduced</span> fraction represented by 2 space-separated integers. The fraction itself should be maximized and if there are several possible ways, you should maximize the denominator. See the samples for a better understanding.</p>





```input1
3
1 2 3
1 2
1 3
```




```input2
1
-2
```




```input3
3
-1 -1 -1
1 2
2 3
```




```input4
3
-1 -2 -1
1 2
1 3
```




```output1
6 1
```




```output2
-2 1
```




```output3
-3 3
```




```output4
-2 2
```



## Note

<p>A connected component is a set of nodes such that for any node in the set, you can reach all other nodes in the set passing only nodes in the set.</p><p>In the first sample, it's optimal to choose the whole tree.</p><p>In the second sample, you only have one choice (to choose node 1) because you can't choose 0 components.</p><p>In the third sample, notice that we could've, for example, chosen only node 1, or node 1 and node 3, or even the whole tree, and the fraction would've had the same value (-1), but we want to maximize $k$. </p><p>In the fourth sample, we'll just choose nodes 1 and 3.</p>
