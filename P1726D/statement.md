## Description

<div><p>You are given a connected, undirected and unweighted graph with $n$ vertices and $m$ edges. Notice <span class="tex-font-style-bf">the limit on the number of edges</span>: $m \le n + 2$.</p><p>Let's say we color some of the edges red and the remaining edges blue. Now consider only the red edges and count the number of connected components in the graph. Let this value be $c_1$. Similarly, consider only the blue edges and count the number of connected components in the graph. Let this value be $c_2$.</p><p>Find an assignment of colors to the edges such that the quantity $c_1+c_2$ is <span class="tex-font-style-bf">minimised</span>.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $n-1 \leq m \leq \min{\left(n+2,\frac{n \cdot (n-1)}{2}\right)}$)&nbsp;— the number of vertices and the number of edges respectively.</p><p>$m$ lines follow. The $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i,v_i \le n$, $u_i \ne v_i$) denoting that the $i$-th edge goes between vertices $u_i$ and $v_i$. The input is guaranteed to have no multiple edges or self loops. The graph is also guaranteed to be connected.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. It is guaranteed that the sum of $m$ over all test cases does not exceed $2 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output a binary string of length $m$. The $i$-th character of the string should be <span class="tex-font-style-tt">1</span> if the $i$-th edge should be colored red, and <span class="tex-font-style-tt">0</span> if it should be colored blue. If there are multiple ways to assign colors to edges that give the minimum answer, you may output any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$; $n-1 \leq m \leq \min{\left(n+2,\frac{n \cdot (n-1)}{2}\right)}$)&nbsp;— the number of vertices and the number of edges respectively.</p><p>$m$ lines follow. The $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i,v_i \le n$, $u_i \ne v_i$) denoting that the $i$-th edge goes between vertices $u_i$ and $v_i$. The input is guaranteed to have no multiple edges or self loops. The graph is also guaranteed to be connected.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$. It is guaranteed that the sum of $m$ over all test cases does not exceed $2 \cdot 10^6$.</p>

## Output

<p>For each test case, output a binary string of length $m$. The $i$-th character of the string should be <span class="tex-font-style-tt">1</span> if the $i$-th edge should be colored red, and <span class="tex-font-style-tt">0</span> if it should be colored blue. If there are multiple ways to assign colors to edges that give the minimum answer, you may output any.</p>





```input1|2,3,4,5,6,7,8,9,15,16,17,18,19,20,21,22
4
5 7
1 2
2 3
3 4
4 5
5 1
1 3
3 5
4 4
1 2
2 3
1 4
3 4
6 7
1 2
1 3
3 4
4 5
1 4
5 6
6 2
2 1
1 2
```




```output1
0111010
1001
0001111
0
```



## Note

<ul><li> The corresponding graph of the first test case is:<center> <img class="tex-graphics" src="file://fgH3iOIZ.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center><p>$c_1 + c_2 = 1 + 2 = 3$</p></li><li> The corresponding graph of the second test case is:<center> <img class="tex-graphics" src="file://WiXpcCFn.png" style="max-width: 100.0%;max-height: 100.0%;" width="189px"> </center><p>$c_1 + c_2 = 2 + 2 = 4$</p></li></ul>
