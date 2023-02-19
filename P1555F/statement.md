## Description

<div><p>You have an undirected graph consisting of $n$ vertices with weighted edges.</p><p>A simple cycle is a cycle of the graph without repeated vertices. Let the <span class="tex-font-style-it">weight</span> of the cycle be the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">XOR</a> of weights of edges it consists of.</p><p>Let's say the graph is <span class="tex-font-style-it">good</span> if all its <span class="tex-font-style-it">simple</span> cycles have weight $1$. A graph is bad if it's not good.</p><p>Initially, the graph is empty. Then $q$ queries follow. Each query has the next type: </p><ul> <li> $u$ $v$ $x$&nbsp;— add edge between vertices $u$ and $v$ of weight $x$ if it doesn't make the graph bad. </li></ul><p>For each query print, was the edge added or not.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($3 \le n \le 3 \cdot 10^5$; $1 \le q \le 5 \cdot 10^5$)&nbsp;— the number of vertices and queries.</p><p>Next $q$ lines contain queries&nbsp;— one per line. Each query contains three integers $u$, $v$ and $x$ ($1 \le u, v \le n$; $u \neq v$; $0 \le x \le 1$)&nbsp;— the vertices of the edge and its weight.</p><p><span class="tex-font-style-bf">It's guaranteed that there are no multiple edges in the input.</span></p></div><div class="output-specification"><p>For each query, print <span class="tex-font-style-tt">YES</span> if the edge was added to the graph, or <span class="tex-font-style-tt">NO</span> otherwise (both case-insensitive).</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($3 \le n \le 3 \cdot 10^5$; $1 \le q \le 5 \cdot 10^5$)&nbsp;— the number of vertices and queries.</p><p>Next $q$ lines contain queries&nbsp;— one per line. Each query contains three integers $u$, $v$ and $x$ ($1 \le u, v \le n$; $u \neq v$; $0 \le x \le 1$)&nbsp;— the vertices of the edge and its weight.</p><p><span class="tex-font-style-bf">It's guaranteed that there are no multiple edges in the input.</span></p>

## Output

<p>For each query, print <span class="tex-font-style-tt">YES</span> if the edge was added to the graph, or <span class="tex-font-style-tt">NO</span> otherwise (both case-insensitive).</p>





```input1
9 12
6 1 0
1 3 1
3 6 0
6 2 0
6 4 1
3 4 1
2 4 0
2 5 0
4 5 0
7 8 1
8 9 1
9 7 0
```




```output1
YES
YES
YES
YES
YES
NO
YES
YES
NO
YES
YES
NO
```


