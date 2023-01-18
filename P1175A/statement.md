## Description

<div><p>You are given an integer $n$ and an integer $k$.</p><p>In one step you can do one of the following moves: </p><ul> <li> decrease $n$ by $1$; </li><li> divide $n$ by $k$ if $n$ is divisible by $k$. </li></ul><p>For example, if $n = 27$ and $k = 3$ you can do the following steps: $27 \rightarrow 26 \rightarrow 25 \rightarrow 24 \rightarrow 8 \rightarrow 7 \rightarrow 6 \rightarrow 2 \rightarrow 1 \rightarrow 0$.</p><p>You are asked to calculate the minimum number of steps to reach $0$ from $n$. </p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of queries.</p><p>The only line of each query contains two integers $n$ and $k$ ($1 \le n \le 10^{18}$, $2 \le k \le 10^{18}$).</p></div><div class="output-specification"><p>For each query print the minimum number of steps to reach $0$ from $n$ in single line. </p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of queries.</p><p>The only line of each query contains two integers $n$ and $k$ ($1 \le n \le 10^{18}$, $2 \le k \le 10^{18}$).</p>

## Output

<p>For each query print the minimum number of steps to reach $0$ from $n$ in single line. </p>





```input1
2
59 3
1000000000000000000 10
```




```output1
8
19
```



## Note

<p>Steps for the first test case are: $59 \rightarrow 58 \rightarrow 57 \rightarrow 19 \rightarrow 18 \rightarrow 6 \rightarrow 2 \rightarrow 1 \rightarrow 0$.</p><p>In the second test case you have to divide $n$ by $k$ $18$ times and then decrease $n$ by $1$.</p>
