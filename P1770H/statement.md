## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Wow, what a big face!</span></div><div class="epigraph-source"><span class="tex-font-style-it"><span class="tex-font-size-small">Kagura Mahiru</span></span></div></div><p>Koxia and Mahiru are enjoying the Winter Festival. The streets of the Winter Festival can be represented as a $n \times n$ undirected grid graph. Formally, the set of vertices is $\{(i,j) \; | \; 1 \leq i,j\leq n \}$ and two vertices $(i_1,j_1)$ and $(i_2,j_2)$ are connected by an edge if and only if $|i_1-i_2|+|j_1-j_2|=1$.</p><center> <img class="tex-graphics" src="file://0xfNAFsX.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"> <span class="tex-font-size-small">A network with size $n = 3$.</span> </center><p>Koxia and Mahiru are planning to visit The Winter Festival by traversing $2n$ routes. Although routes are not planned yet, the endpoints of the routes are already planned as follows:</p><ul> <li> In the $i$-th route, they want to start from vertex $(1, i)$ and end at vertex $(n, p_i)$, where $p$ is a permutation of length $n$. </li><li> In the $(i+n)$-th route, they want to start from vertex $(i, 1)$ and end at vertex $(q_i, n)$, where $q$ is a permutation of length $n$. </li></ul><center> <img class="tex-graphics" src="file://Ad9eqB5D.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> <span class="tex-font-size-small">A network with size $n = 3$, points to be connected are shown in the same color for $p = [3, 2, 1]$ and $q = [3, 1, 2]$.</span> </center><p>Your task is to find a routing scheme — $2n$ paths where each path connects the specified endpoints. Let's define the <span class="tex-font-style-it">congestion</span> of an edge as the number of times it is used (both directions combined) in the routing scheme. In order to ensure that Koxia and Mahiru won't get too bored because of traversing repeated edges, please find a routing scheme that <span class="tex-font-style-bf">minimizes the maximum congestion among all edges</span>.</p><center> <img class="tex-graphics" src="file://roTIm9WL.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> <span class="tex-font-size-small">An example solution — the maximum congestion is $2$, which is optimal in this case.</span> </center></div><div class="input-specification"><p>The first line contains an integer $n$ ($2 \leq n \leq 200$) — the size of the network. </p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \leq p_i \leq n$).</p><p>The third line contains $n$ integers $q_1, q_2, \dots, q_n$ ($1 \leq q_i \leq n$).</p><p>It is guaranteed that both $p$ and $q$ are permutations of length $n$.</p></div><div class="output-specification"><p>Output $2n$ lines, each line describing a route.</p><p>The first $n$ lines should describe the connections from top to bottom. The $i$-th line should describe the route starting at vertex $(1, i)$ and ending at vertex $(n, p_i)$.</p><p>The next $n$ lines should describe the connections from left to right. The $(i+n)$-th line should describe the route starting at vertex $(i, 1)$ and ending at vertex $(q_i, n)$.</p><p>Each line describing a route should start with an integer $k$ ($2 \le k \le 10^5$) — the number of vertices the route passes, including the starting and ending vertices. Then output all the vertices on the route in order. In other words, if the route is $(x_1, y_1) \rightarrow (x_2, y_2) \rightarrow \dots \rightarrow (x_k, y_k)$, then output $k~x_1~y_1~x_2~y_2 \ldots x_k~y_k$. Note that $|x_i-x_{i+1}|+|y_i-y_{i+1}| = 1$ should holds for $1 \le i &lt; k$.</p><p>If there are multiple solutions that minimize the maximum congestion, you may output any.</p></div>

## Input

<p>The first line contains an integer $n$ ($2 \leq n \leq 200$) — the size of the network. </p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \leq p_i \leq n$).</p><p>The third line contains $n$ integers $q_1, q_2, \dots, q_n$ ($1 \leq q_i \leq n$).</p><p>It is guaranteed that both $p$ and $q$ are permutations of length $n$.</p>

## Output

<p>Output $2n$ lines, each line describing a route.</p><p>The first $n$ lines should describe the connections from top to bottom. The $i$-th line should describe the route starting at vertex $(1, i)$ and ending at vertex $(n, p_i)$.</p><p>The next $n$ lines should describe the connections from left to right. The $(i+n)$-th line should describe the route starting at vertex $(i, 1)$ and ending at vertex $(q_i, n)$.</p><p>Each line describing a route should start with an integer $k$ ($2 \le k \le 10^5$) — the number of vertices the route passes, including the starting and ending vertices. Then output all the vertices on the route in order. In other words, if the route is $(x_1, y_1) \rightarrow (x_2, y_2) \rightarrow \dots \rightarrow (x_k, y_k)$, then output $k~x_1~y_1~x_2~y_2 \ldots x_k~y_k$. Note that $|x_i-x_{i+1}|+|y_i-y_{i+1}| = 1$ should holds for $1 \le i &lt; k$.</p><p>If there are multiple solutions that minimize the maximum congestion, you may output any.</p>





```input1
3
3 2 1
3 1 2
```




```input2
4
3 4 2 1
2 4 1 3
```




```input3
3
1 2 3
1 2 3
```




```output1
5 1 1 2 1 2 2 3 2 3 3 
3 1 2 2 2 3 2 
5 1 3 1 2 1 1 2 1 3 1 
5 1 1 1 2 1 3 2 3 3 3
4 2 1 2 2 2 3 1 3 
4 3 1 3 2 3 3 2 3
```




```output2
6 1 1 1 2 2 2 2 3 3 3 4 3
6 1 2 1 3 2 3 2 4 3 4 4 4
5 1 3 2 3 2 2 3 2 4 2
7 1 4 1 3 1 2 2 2 2 1 3 1 4 1
7 1 1 2 1 3 1 3 2 3 3 2 3 2 4
6 2 1 2 2 3 2 4 2 4 3 4 4
6 3 1 3 2 3 3 3 4 2 4 1 4
5 4 1 4 2 4 3 3 3 3 4
```




```output3
3 1 1 2 1 3 1 
3 1 2 2 2 3 2 
3 1 3 2 3 3 3 
3 1 1 1 2 1 3 
3 2 1 2 2 2 3 
3 3 1 3 2 3 3
```



## Note

<p>The first example corresponds to the figures in the problem statement.</p><p>The output for examples $2$ and $3$ respectively are visualized below:</p><center> <img class="tex-graphics" src="file://OSnlTDag.png" style="max-width: 100.0%;max-height: 100.0%;" width="643px"> <span class="tex-font-size-small">Sample output for examples $2$ and $3$. Maximum congestions are $2$ and $1$ respectively.</span> </center>
