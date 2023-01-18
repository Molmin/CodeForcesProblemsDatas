## Description

<div><p><span class="tex-font-style-it">The main characters have been omitted to be short.</span></p><p>You are given a directed unweighted graph without loops with $n$ vertexes and a path in it (that path is not necessary simple) given by a sequence $p_1, p_2, \ldots, p_m$ of $m$ vertexes; for each $1 \leq i &lt; m$ there is an arc from $p_i$ to $p_{i+1}$.</p><p>Define the sequence $v_1, v_2, \ldots, v_k$ of $k$ vertexes as <span class="tex-font-style-it">good</span>, if $v$ is a subsequence of $p$, $v_1 = p_1$, $v_k = p_m$, and $p$ is one of the shortest paths passing through the vertexes $v_1$, $\ldots$, $v_k$ in that order.</p><p>A sequence $a$ is a subsequence of a sequence $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements. It is obvious that the sequence $p$ is good but your task is to find the <span class="tex-font-style-bf">shortest</span> good subsequence.</p><p>If there are multiple shortest good subsequences, output any of them.</p><p> </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the number of vertexes in a graph. </p><p>The next $n$ lines define the graph by an adjacency matrix: the $j$-th character in the $i$-st line is equal to $1$ if there is an arc from vertex $i$ to the vertex $j$ else it is equal to $0$. It is guaranteed that the graph doesn't contain loops.</p><p>The next line contains a single integer $m$ ($2 \le m \le 10^6$)&nbsp;— the number of vertexes in the path. </p><p>The next line contains $m$ integers $p_1, p_2, \ldots, p_m$ ($1 \le p_i \le n$)&nbsp;— the sequence of vertexes in the path. It is guaranteed that for any $1 \leq i &lt; m$ there is an arc from $p_i$ to $p_{i+1}$.</p></div><div class="output-specification"><p>In the first line output a single integer $k$ ($2 \leq k \leq m$)&nbsp;— the length of the shortest good subsequence. In the second line output $k$ integers $v_1$, $\ldots$, $v_k$ ($1 \leq v_i \leq n$)&nbsp;— the vertexes in the subsequence. If there are multiple shortest subsequences, print any. Any two consecutive numbers should be distinct.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the number of vertexes in a graph. </p><p>The next $n$ lines define the graph by an adjacency matrix: the $j$-th character in the $i$-st line is equal to $1$ if there is an arc from vertex $i$ to the vertex $j$ else it is equal to $0$. It is guaranteed that the graph doesn't contain loops.</p><p>The next line contains a single integer $m$ ($2 \le m \le 10^6$)&nbsp;— the number of vertexes in the path. </p><p>The next line contains $m$ integers $p_1, p_2, \ldots, p_m$ ($1 \le p_i \le n$)&nbsp;— the sequence of vertexes in the path. It is guaranteed that for any $1 \leq i &lt; m$ there is an arc from $p_i$ to $p_{i+1}$.</p>

## Output

<p>In the first line output a single integer $k$ ($2 \leq k \leq m$)&nbsp;— the length of the shortest good subsequence. In the second line output $k$ integers $v_1$, $\ldots$, $v_k$ ($1 \leq v_i \leq n$)&nbsp;— the vertexes in the subsequence. If there are multiple shortest subsequences, print any. Any two consecutive numbers should be distinct.</p>





```input1
4
0110
0010
0001
1000
4
1 2 3 4
```




```input2
4
0110
0010
1001
1000
20
1 2 3 4 1 2 3 4 1 2 3 4 1 2 3 4 1 2 3 4
```




```input3
3
011
101
110
7
1 2 3 1 3 2 1
```




```input4
4
0110
0001
0001
1000
3
1 2 4
```




```output1
3
1 2 4
```




```output2
11
1 2 4 2 4 2 4 2 4 2 4
```




```output3
7
1 2 3 1 3 2 1
```




```output4
2
1 4
```



## Note

<p>Below you can see the graph from the first example:</p><p><img class="tex-graphics" src="file://Uvabu0K7.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The given path is passing through vertexes $1$, $2$, $3$, $4$. The sequence $1-2-4$ is good because it is the subsequence of the given path, its first and the last elements are equal to the first and the last elements of the given path respectively, and the shortest path passing through vertexes $1$, $2$ and $4$ in that order is $1-2-3-4$. Note that subsequences $1-4$ and $1-3-4$ aren't good because in both cases the shortest path passing through the vertexes of these sequences is $1-3-4$.</p><p>In the third example, the graph is full so any sequence of vertexes in which any two consecutive elements are distinct defines a path consisting of the same number of vertexes.</p><p>In the fourth example, the paths $1-2-4$ and $1-3-4$ are the shortest paths passing through the vertexes $1$ and $4$.</p>
