## Description

<div><p>In this problem, we will consider <span class="tex-font-style-bf">complete</span> undirected graphs consisting of $n$ vertices with weighted edges. The weight of each edge is an integer from $1$ to $k$.</p><p>An undirected graph is considered <span class="tex-font-style-bf">beautiful</span> if the sum of weights of all edges incident to vertex $1$ is equal to the weight of MST in the graph. MST is the minimum spanning tree&nbsp;— a tree consisting of $n-1$ edges of the graph, which connects all $n$ vertices and has the minimum sum of weights among all such trees; the weight of MST is the sum of weights of all edges in it.</p><p>Calculate the number of <span class="tex-font-style-bf">complete</span> <span class="tex-font-style-bf">beautiful</span> graphs having exactly $n$ vertices and the weights of edges from $1$ to $k$. Since the answer might be large, print it modulo $998244353$.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $k$ ($2 \le n \le 250$; $1 \le k \le 250$).</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of <span class="tex-font-style-bf">complete</span> <span class="tex-font-style-bf">beautiful</span> graphs having exactly $n$ vertices and the weights of edges from $1$ to $k$. Since the answer might be large, print it modulo $998244353$.</p></div>

## Input

<p>The only line contains two integers $n$ and $k$ ($2 \le n \le 250$; $1 \le k \le 250$).</p>

## Output

<p>Print one integer&nbsp;— the number of <span class="tex-font-style-bf">complete</span> <span class="tex-font-style-bf">beautiful</span> graphs having exactly $n$ vertices and the weights of edges from $1$ to $k$. Since the answer might be large, print it modulo $998244353$.</p>





```input1
3 2
```




```input2
4 4
```




```input3
6 9
```




```input4
42 13
```




```output1
5
```




```output2
571
```




```output3
310640163
```




```output4
136246935
```


