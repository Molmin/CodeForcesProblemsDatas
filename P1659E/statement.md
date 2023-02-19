## Description

<div><p>There is an undirected, connected graph with $n$ vertices and $m$ weighted edges. A <span class="tex-font-style-it">walk</span> from vertex $u$ to vertex $v$ is defined as a sequence of vertices $p_1,p_2,\ldots,p_k$ (which are not necessarily distinct) starting with $u$ and ending with $v$, such that $p_i$ and $p_{i+1}$ are connected by an edge for $1 \leq i &lt; k$.</p><p>We define the <span class="tex-font-style-it">length</span> of a walk as follows: take the ordered sequence of edges and write down the weights on each of them in an array. Now, write down the bitwise AND of every nonempty prefix of this array. The <span class="tex-font-style-it">length</span> of the walk is the MEX of all these values.</p><p>More formally, let us have $[w_1,w_2,\ldots,w_{k-1}]$ where $w_i$ is the weight of the edge between $p_i$ and $p_{i+1}$. Then the <span class="tex-font-style-it">length</span> of the walk is given by $\mathrm{MEX}(\{w_1,\,w_1\&amp; w_2,\,\ldots,\,w_1\&amp; w_2\&amp; \ldots\&amp; w_{k-1}\})$, where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>Now you must process $q$ queries of the form <span class="tex-font-style-tt">u v</span>. For each query, find the <span class="tex-font-style-bf">minimum</span> possible length of a walk from $u$ to $v$.</p><p>The MEX (minimum excluded) of a set is the smallest non-negative integer that does not belong to the set. For instance: </p><ul> <li> The MEX of $\{2,1\}$ is $0$, because $0$ does not belong to the set. </li><li> The MEX of $\{3,1,0\}$ is $2$, because $0$ and $1$ belong to the set, but $2$ does not. </li><li> The MEX of $\{0,3,1,2\}$ is $4$ because $0$, $1$, $2$ and $3$ belong to the set, but $4$ does not. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \leq n \leq 10^5$; $n-1 \leq m \leq \min{\left(\frac{n(n-1)}{2},10^5\right)}$).</p><p>Each of the next $m$ lines contains three integers $a$, $b$, and $w$ ($1 \leq a, b \leq n$, $a \neq b$; $0 \leq w &lt; 2^{30}$) indicating an undirected edge between vertex $a$ and vertex $b$ with weight $w$. The input will not contain self-loops or duplicate edges, and the provided graph will be connected.</p><p>The next line contains a single integer $q$ ($1 \leq q \leq 10^5$).</p><p>Each of the next $q$ lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n$, $u \neq v$), the description of each query.</p></div><div class="output-specification"><p>For each query, print one line containing a single integer&nbsp;— the answer to the query.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \leq n \leq 10^5$; $n-1 \leq m \leq \min{\left(\frac{n(n-1)}{2},10^5\right)}$).</p><p>Each of the next $m$ lines contains three integers $a$, $b$, and $w$ ($1 \leq a, b \leq n$, $a \neq b$; $0 \leq w &lt; 2^{30}$) indicating an undirected edge between vertex $a$ and vertex $b$ with weight $w$. The input will not contain self-loops or duplicate edges, and the provided graph will be connected.</p><p>The next line contains a single integer $q$ ($1 \leq q \leq 10^5$).</p><p>Each of the next $q$ lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n$, $u \neq v$), the description of each query.</p>

## Output

<p>For each query, print one line containing a single integer&nbsp;— the answer to the query.</p>





```input1
6 7
1 2 1
2 3 3
3 1 5
4 5 2
5 6 4
6 4 6
3 4 1
3
1 5
1 2
5 3
```




```input2
9 8
1 2 5
2 3 11
3 4 10
3 5 10
5 6 2
5 7 1
7 8 5
7 9 5
10
5 7
2 5
7 1
6 4
5 2
7 6
4 1
6 2
4 7
2 8
```




```output1
2
0
1
```




```output2
0
0
2
0
0
2
1
0
1
1
```



## Note

<p>The following is an explanation of the first example.</p><center> <img class="tex-graphics" src="file://toaHS5w4.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The graph in the first example.</span> </center><p>Here is one possible walk for the first query:</p><p>$$1 \overset{5}{\rightarrow} 3 \overset{3}{\rightarrow} 2 \overset{1}{\rightarrow} 1 \overset{5}{\rightarrow} 3 \overset{1}{\rightarrow} 4 \overset{2}{\rightarrow} 5.$$</p><p>The array of weights is $w=[5,3,1,5,1,2]$. Now if we take the bitwise AND of every prefix of this array, we get the set $\{5,1,0\}$. The MEX of this set is $2$. We cannot get a walk with a smaller length (as defined in the statement).</p>
