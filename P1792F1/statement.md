## Description

<div><p><span class="tex-font-style-bf">The only difference between the easy and the hard version is the constraint on $n$.</span></p><p>You are given an undirected complete graph on $n$ vertices. A complete graph is a graph where each pair of vertices is connected by an edge. You have to paint the edges of the graph into two colors, red and blue (each edge will have one color).</p><p>A set of vertices $S$ is <span class="tex-font-style-bf">red-connected</span> if, for every pair of vertices $(v_1, v_2)$ such that $v_1 \in S$ and $v_2 \in S$, there exists a path from $v_1$ to $v_2$ that goes only through red edges and vertices from $S$. Similarly, a set of vertices $S$ is <span class="tex-font-style-bf">blue-connected</span> if, for every pair of vertices $(v_1, v_2)$ such that $v_1 \in S$ and $v_2 \in S$, there exists a path from $v_1$ to $v_2$ that goes only through blue edges and vertices from $S$.</p><p>You have to paint the graph in such a way that:</p><ul> <li> there is at least one red edge; </li><li> there is at least one blue edge; </li><li> for each set of vertices $S$ such that $|S| \ge 2$, $S$ is either red-connected or blue-connected, but <span class="tex-font-style-bf">not both</span>. </li></ul><p>Calculate the number of ways to paint the graph, and print it modulo $998244353$.</p></div><div class="input-specification"><p>The first (and only) line contains one integer $n$ ($3 \le n \le 5 \cdot 10^3$).</p></div><div class="output-specification"><p>Print one integer — the number of ways to paint the graph, taken modulo $998244353$.</p></div>

## Input

<p>The first (and only) line contains one integer $n$ ($3 \le n \le 5 \cdot 10^3$).</p>

## Output

<p>Print one integer — the number of ways to paint the graph, taken modulo $998244353$.</p>





```input1
3
```




```input2
4
```




```input3
100
```




```input4
1337
```




```output1
6
```




```output2
50
```




```output3
878752271
```




```output4
520628749
```


