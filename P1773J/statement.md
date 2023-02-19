## Description

<div><p>You are given an undirected connected graph with $n$ vertices and $m$ edges. Each edge has an associated counter, initially equal to $0$. In one operation, you can choose an arbitrary spanning tree and add any value $v$ to all edges of this spanning tree. </p><p>Determine if it's possible to make every counter equal to its target value $x_i$ modulo prime $p$, and provide a sequence of operations that achieves it.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $p$&nbsp;— the number of vertices, the number of edges, and the prime modulus ($1 \le n \le 500$; $1 \le m \le 1000$; $2 \le p \le 10^9$, $p$ is prime).</p><p>Next $m$ lines contain three integers $u_i$, $v_i$, $x_i$ each&nbsp;— the two endpoints of the $i$-th edge and the target value of that edge's counter ($1 \le u_i, v_i \le n$; $0 \le x_i &lt; p$; $u_i \neq v_i$). </p><p>The graph is connected. There are no loops, but there may be multiple edges between the same two vertices.</p></div><div class="output-specification"><p>If the target values on counters cannot be achieved, print <span class="tex-font-style-tt">-1</span>. </p><p>Otherwise, print $t$&nbsp;— the number of operations, followed by $t$ lines, describing the sequence of operations. Each line starts with integer $v$ ($0 \le v &lt; p$)&nbsp;— the counter increment for this operation. Then, in the same line, followed by $n - 1$ integers $e_1$, $e_2$, ... $e_{n - 1}$ ($1 \le e_i \le m$)&nbsp;— the edges of the spanning tree.</p><p>The number of operations $t$ should not exceed $2m$. You don't need to minimize $t$. Any correct answer within the $2m$ bound is accepted. You are allowed to repeat spanning trees.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $p$&nbsp;— the number of vertices, the number of edges, and the prime modulus ($1 \le n \le 500$; $1 \le m \le 1000$; $2 \le p \le 10^9$, $p$ is prime).</p><p>Next $m$ lines contain three integers $u_i$, $v_i$, $x_i$ each&nbsp;— the two endpoints of the $i$-th edge and the target value of that edge's counter ($1 \le u_i, v_i \le n$; $0 \le x_i &lt; p$; $u_i \neq v_i$). </p><p>The graph is connected. There are no loops, but there may be multiple edges between the same two vertices.</p>

## Output

<p>If the target values on counters cannot be achieved, print <span class="tex-font-style-tt">-1</span>. </p><p>Otherwise, print $t$&nbsp;— the number of operations, followed by $t$ lines, describing the sequence of operations. Each line starts with integer $v$ ($0 \le v &lt; p$)&nbsp;— the counter increment for this operation. Then, in the same line, followed by $n - 1$ integers $e_1$, $e_2$, ... $e_{n - 1}$ ($1 \le e_i \le m$)&nbsp;— the edges of the spanning tree.</p><p>The number of operations $t$ should not exceed $2m$. You don't need to minimize $t$. Any correct answer within the $2m$ bound is accepted. You are allowed to repeat spanning trees.</p>





```input1
3 3 101
1 2 30
2 3 40
3 1 50
```




```input2
2 2 37
1 2 8
1 2 15
```




```input3
5 4 5
1 3 1
2 3 2
2 5 3
4 1 4
```




```output1
3
10 1 2
20 1 3
30 2 3
```




```output2
2
8 1
15 2
```




```output3
-1
```


