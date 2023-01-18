## Description

<div><p>Every person likes prime numbers. Alice is a person, thus she also shares the love for them. Bob wanted to give her an affectionate gift but couldn't think of anything inventive. Hence, he will be giving her a graph. How original, Bob! Alice will surely be <span class="tex-font-style-it">thrilled</span>!</p><p>When building the graph, he needs four conditions to be satisfied: </p><ul> <li> It must be a simple undirected graph, i.e. without multiple (parallel) edges and self-loops. </li><li> The number of vertices must be exactly $n$&nbsp;— a number he selected. This number is not necessarily prime. </li><li> The total number of edges must be prime. </li><li> The degree (i.e. the number of edges connected to the vertex) of each vertex must be prime. </li></ul><p>Below is an example for $n = 4$. The first graph (left one) is invalid as the degree of vertex $2$ (and $4$) equals to $1$, which is not prime. The second graph (middle one) is invalid as the total number of edges is $4$, which is not a prime number. The third graph (right one) is a valid answer for $n = 4$. </p><center> <img class="tex-graphics" src="file://KgMxlsSF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Note that the graph can be disconnected.</p><p>Please help Bob to find any such graph!</p></div><div class="input-specification"><p>The input consists of a single integer $n$ ($3 \leq n \leq 1\,000$)&nbsp;— the number of vertices.</p></div><div class="output-specification"><p>If there is no graph satisfying the conditions, print a single line containing the integer $-1$.</p><p>Otherwise, first print a line containing a prime number $m$ ($2 \leq m \leq \frac{n(n-1)}{2}$)&nbsp;— the number of edges in the graph. Then, print $m$ lines, the $i$-th of which containing two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n$)&nbsp;— meaning that there is an edge between vertices $u_i$ and $v_i$. The degree of each vertex must be prime. There must be no multiple (parallel) edges or self-loops.</p><p>If there are multiple solutions, you may print any of them.</p><p>Note that the graph can be disconnected.</p></div>

## Input

<p>The input consists of a single integer $n$ ($3 \leq n \leq 1\,000$)&nbsp;— the number of vertices.</p>

## Output

<p>If there is no graph satisfying the conditions, print a single line containing the integer $-1$.</p><p>Otherwise, first print a line containing a prime number $m$ ($2 \leq m \leq \frac{n(n-1)}{2}$)&nbsp;— the number of edges in the graph. Then, print $m$ lines, the $i$-th of which containing two integers $u_i$, $v_i$ ($1 \leq u_i, v_i \leq n$)&nbsp;— meaning that there is an edge between vertices $u_i$ and $v_i$. The degree of each vertex must be prime. There must be no multiple (parallel) edges or self-loops.</p><p>If there are multiple solutions, you may print any of them.</p><p>Note that the graph can be disconnected.</p>





```input1
4
```




```input2
8
```




```output1
5
1 2
1 3
2 3
2 4
3 4
```




```output2
13
1 2
1 3
2 3
1 4
2 4
1 5
2 5
1 6
2 6
1 7
1 8
5 8
7 8
```



## Note

<p>The first example was described in the statement.</p><p>In the second example, the degrees of vertices are $[7, 5, 2, 2, 3, 2, 2, 3]$. Each of these numbers is prime. Additionally, the number of edges, $13$, is also a prime number, hence both conditions are satisfied.</p><center> <img class="tex-graphics" src="file://lKE04VGO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
