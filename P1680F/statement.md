## Description

<div><p>You are given a simple connected undirected graph, consisting of $n$ vertices and $m$ edges. The vertices are numbered from $1$ to $n$.</p><p>A vertex cover of a graph is a set of vertices such that each edge has at least one of its endpoints in the set.</p><p>Let's call a <span class="tex-font-style-it">lenient</span> vertex cover such a vertex cover that <span class="tex-font-style-bf">at most one</span> edge in it has both endpoints in the set.</p><p>Find a <span class="tex-font-style-it">lenient</span> vertex cover of a graph or report that there is none. If there are multiple answers, then print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($2 \le n \le 10^6$; $n - 1 \le m \le \min(10^6, \frac{n \cdot (n - 1)}{2})$)&nbsp;— the number of vertices and the number of edges of the graph.</p><p>Each of the next $m$ lines contains two integers $v$ and $u$ ($1 \le v, u \le n$; $v \neq u$)&nbsp;— the descriptions of the edges.</p><p>For each testcase, the graph is connected and doesn't have multiple edges. The sum of $n$ over all testcases doesn't exceed $10^6$. The sum of $m$ over all testcases doesn't exceed $10^6$.</p></div><div class="output-specification"><p>For each testcase, the first line should contain <span class="tex-font-style-tt">YES</span> if a <span class="tex-font-style-it">lenient</span> vertex cover exists, and <span class="tex-font-style-tt">NO</span> otherwise. If it exists, the second line should contain a binary string $s$ of length $n$, where $s_i = 1$ means that vertex $i$ is in the vertex cover, and $s_i = 0$ means that vertex $i$ isn't.</p><p>If there are multiple answers, then print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($2 \le n \le 10^6$; $n - 1 \le m \le \min(10^6, \frac{n \cdot (n - 1)}{2})$)&nbsp;— the number of vertices and the number of edges of the graph.</p><p>Each of the next $m$ lines contains two integers $v$ and $u$ ($1 \le v, u \le n$; $v \neq u$)&nbsp;— the descriptions of the edges.</p><p>For each testcase, the graph is connected and doesn't have multiple edges. The sum of $n$ over all testcases doesn't exceed $10^6$. The sum of $m$ over all testcases doesn't exceed $10^6$.</p>

## Output

<p>For each testcase, the first line should contain <span class="tex-font-style-tt">YES</span> if a <span class="tex-font-style-it">lenient</span> vertex cover exists, and <span class="tex-font-style-tt">NO</span> otherwise. If it exists, the second line should contain a binary string $s$ of length $n$, where $s_i = 1$ means that vertex $i$ is in the vertex cover, and $s_i = 0$ means that vertex $i$ isn't.</p><p>If there are multiple answers, then print any of them.</p>





```input1
4
6 5
1 3
2 4
3 4
3 5
4 6
4 6
1 2
2 3
3 4
1 4
1 3
2 4
8 11
1 3
2 4
3 5
4 6
5 7
6 8
1 2
3 4
5 6
7 8
7 2
4 5
1 2
2 3
3 4
1 3
2 4
```




```input2
1
10 15
9 4
3 4
6 4
1 2
8 2
8 3
7 2
9 5
7 8
5 10
1 4
2 10
5 3
5 7
2 9
```




```input3
1
10 19
7 9
5 3
3 4
1 6
9 4
1 4
10 5
7 1
9 2
8 3
7 3
10 9
2 10
9 8
3 2
1 5
10 7
9 5
1 2
```




```output1
YES
001100
NO
YES
01100110
YES
0110
```




```output2
YES
0101100100
```




```output3
YES
1010000011
```



## Note

<p>Here are the graphs from the first example. The vertices in the <span class="tex-font-style-it">lenient</span> vertex covers are marked red. </p><center> <img class="tex-graphics" src="file://z6iwcKc0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
