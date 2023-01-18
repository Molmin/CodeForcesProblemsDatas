## Description

<div><p>Fedor runs for president of Byteland! In the debates, he will be asked how to solve Byteland's transport problem. It's a really hard problem because of Byteland's transport system is now a tree (connected graph without cycles). Fedor's team has found out in the ministry of transport of Byteland that there is money in the budget only for one additional road. In the debates, he is going to say that he will build this road as a way to maximize the number of distinct simple paths in the country. A simple path is a path which goes through every vertex no more than once. Two simple paths are named distinct if sets of their edges are distinct. </p><p>But Byteland's science is deteriorated, so Fedor's team hasn't succeeded to find any scientists to answer how many distinct simple paths they can achieve after adding exactly one edge on the transport system?</p><p>Help Fedor to solve it.</p><p>An edge can be added between vertices that are already connected, but it can't be a loop.</p><p>In this problem, we consider only simple paths of length at least two.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \leq n \leq 500\ 000$)&nbsp;— number of vertices in Byteland's transport system.</p><p>Each of the following $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \leq v_i, u_i \leq n$). It's guaranteed that the graph is tree.</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— a maximal number of simple paths that can be achieved after adding one edge.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \leq n \leq 500\ 000$)&nbsp;— number of vertices in Byteland's transport system.</p><p>Each of the following $n - 1$ lines contains two integers $v_i$ and $u_i$ ($1 \leq v_i, u_i \leq n$). It's guaranteed that the graph is tree.</p>

## Output

<p>Print exactly one integer&nbsp;— a maximal number of simple paths that can be achieved after adding one edge.</p>





```input1
2
1 2
```




```input2
4
1 2
1 3
1 4
```




```input3
6
1 2
1 3
3 4
3 5
4 6
```




```output1
2
```




```output2
11
```




```output3
29
```


