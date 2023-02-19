## Description

<div><p>You are given a simple undirected graph, consisting of $n$ vertices and $m$ edges. The vertices are numbered from $1$ to $n$. The $i$-th vertex has a value $a_i$ written on it.</p><p>You will be removing vertices from that graph. You are allowed to remove vertex $i$ only if its degree is equal to $a_i$. When a vertex is removed, all edges incident to it are also removed, thus, decreasing the degree of adjacent non-removed vertices.</p><p>A valid sequence of removals is a permutation $p_1, p_2, \dots, p_n$ $(1 \le p_i \le n)$ such that the $i$-th vertex to be removed is $p_i$, and every removal is allowed.</p><p>A pair $(x, y)$ of vertices is <span class="tex-font-style-it">nice</span> if there exist two valid sequences of removals such that $x$ is removed before $y$ in one of them and $y$ is removed before $x$ in the other one.</p><p>Count the number of <span class="tex-font-style-it">nice</span> pairs $(x, y)$ such that $x &lt; y$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($1 \le n \le 10^5$; $0 \le m \le \min(10^5, \frac{n \cdot (n - 1)}{2})$)&nbsp;— the number of vertices and the number of edges of the graph.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le n - 1$)&nbsp;— the degree requirements for each removal.</p><p>Each of the next $m$ lines contains two integers $v$ and $u$ ($1 \le v, u \le n$; $v \neq u$)&nbsp;— the description of an edge.</p><p>The graph doesn't contain any self-loops or multiple edges.</p><p>The sum of $n$ over all testcases doesn't exceed $10^5$. The sum of $m$ over all testcases doesn't exceed $10^5$.</p><p><span class="tex-font-style-bf">Additional constraint on the input: there always exists at least one valid sequence of removals.</span></p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the number of <span class="tex-font-style-it">nice</span> pairs of vertices.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($1 \le n \le 10^5$; $0 \le m \le \min(10^5, \frac{n \cdot (n - 1)}{2})$)&nbsp;— the number of vertices and the number of edges of the graph.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le n - 1$)&nbsp;— the degree requirements for each removal.</p><p>Each of the next $m$ lines contains two integers $v$ and $u$ ($1 \le v, u \le n$; $v \neq u$)&nbsp;— the description of an edge.</p><p>The graph doesn't contain any self-loops or multiple edges.</p><p>The sum of $n$ over all testcases doesn't exceed $10^5$. The sum of $m$ over all testcases doesn't exceed $10^5$.</p><p><span class="tex-font-style-bf">Additional constraint on the input: there always exists at least one valid sequence of removals.</span></p>

## Output

<p>For each testcase, print a single integer&nbsp;— the number of <span class="tex-font-style-it">nice</span> pairs of vertices.</p>





```input1|2,3,4,5,11,12,13,14,15,16,17,18
4
3 2
1 0 1
2 3
1 2
3 3
1 2 0
1 2
2 3
1 3
5 6
3 0 2 1 0
1 2
4 1
4 2
3 4
2 3
5 1
1 0
0
```




```output1
1
0
4
0
```


