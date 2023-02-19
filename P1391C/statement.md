## Description

<div><p>A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>Consider a permutation $p$ of length $n$, we build a graph of size $n$ using it as follows: </p><ul> <li> For every $1 \leq i \leq n$, find the <span class="tex-font-style-bf">largest</span> $j$ such that $1 \leq j &lt; i$ and $p_j &gt; p_i$, and add an undirected edge between node $i$ and node $j$ </li><li> For every $1 \leq i \leq n$, find the <span class="tex-font-style-bf">smallest</span> $j$ such that $i &lt; j \leq n$ and $p_j &gt; p_i$, and add an undirected edge between node $i$ and node $j$ </li></ul><p>In cases where no such $j$ exists, we make no edges. Also, note that we make edges between the corresponding indices, not the values at those indices.</p><p>For clarity, consider as an example $n = 4$, and $p = [3,1,4,2]$; here, the edges of the graph are $(1,3),(2,1),(2,3),(4,3)$.</p><p>A permutation $p$ is <span class="tex-font-style-bf">cyclic</span> if the graph built using $p$ has at least one simple cycle. </p><p>Given $n$, find the number of cyclic permutations of length $n$. Since the number may be very large, output it modulo $10^9+7$.</p><p>Please refer to the Notes section for the formal definition of a simple cycle</p></div><div class="input-specification"><p>The first and only line contains a single integer $n$ ($3 \le n \le 10^6$).</p></div><div class="output-specification"><p>Output a single integer $0 \leq x &lt; 10^9+7$, the number of cyclic permutations of length $n$ modulo $10^9+7$.</p></div>

## Input

<p>The first and only line contains a single integer $n$ ($3 \le n \le 10^6$).</p>

## Output

<p>Output a single integer $0 \leq x &lt; 10^9+7$, the number of cyclic permutations of length $n$ modulo $10^9+7$.</p>





```input1
4
```




```input2
583291
```




```output1
16
```




```output2
135712853
```



## Note

<p>There are $16$ cyclic permutations for $n = 4$. $[4,2,1,3]$ is one such permutation, having a cycle of length four: $4 \rightarrow 3 \rightarrow 2 \rightarrow 1 \rightarrow 4$.</p><p>Nodes $v_1$, $v_2$, $\ldots$, $v_k$ form a simple cycle if the following conditions hold: </p><ul> <li> $k \geq 3$. </li><li> $v_i \neq v_j$ for any pair of indices $i$ and $j$. ($1 \leq i &lt; j \leq k$) </li><li> $v_i$ and $v_{i+1}$ share an edge for all $i$ ($1 \leq i &lt; k$), and $v_1$ and $v_k$ share an edge. </li></ul>
