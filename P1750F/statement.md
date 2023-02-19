## Description

<div><p>Everyone was happy coding, until suddenly a power shortage happened and the best competitive programming site went down. Fortunately, a system administrator bought some new equipment recently, including some UPSs. Thus there are some servers that are still online, but we need all of them to be working in order to keep the round rated.</p><p>Imagine the servers being a binary string $s$ of length $n$. If the $i$-th server is online, then $s_i = 1$, and $s_i = 0$ otherwise.</p><p>A system administrator can do the following operation called <span class="tex-font-style-it">electricity spread</span>, that consists of the following phases: </p><ul> <li> Select two servers at positions $1 \le i &lt; j \le n$ such that both are online (i.e. $s_i=s_j=1$). The spread starts only from online servers. </li><li> Check if we have enough power to make the spread. We consider having enough power if the number of turned on servers in range $[i, j]$ is at least the number of turned off servers in range $[i, j]$. More formally, check whether $2 \cdot (s_i + s_{i+1} + \ldots + s_j) \ge j - i + 1$.</li><li> If the check is positive, turn on all the offline servers in range $[i, j]$. More formally, make $s_k := 1$ for all $k$ from $i$ to $j$. </li></ul><p>We call a binary string $s$ of length $n$ <span class="tex-font-style-it">rated</span> if we can turn on all servers (i.e. make $s_i = 1$ for $1 \le i \le n$) using the electricity spread operation any number of times (possibly, $0$). Your task is to find the number of rated strings of length $n$ modulo $m$.</p></div><div class="input-specification"><p>The first and only line contains two integers $n$ and $m$ ($1 \le n \le 5000$, $10 \le m \le 10^9$) — the length of the string and the required module.</p></div><div class="output-specification"><p>Print a single integer — the number of rated binary strings of length $n$. Since this number can be large, print it modulo $m$.</p></div>

## Input

<p>The first and only line contains two integers $n$ and $m$ ($1 \le n \le 5000$, $10 \le m \le 10^9$) — the length of the string and the required module.</p>

## Output

<p>Print a single integer — the number of rated binary strings of length $n$. Since this number can be large, print it modulo $m$.</p>





```input1
2 100
```




```input2
3 10
```




```input3
4 3271890
```




```input4
17 123456
```




```output1
1
```




```output2
2
```




```output3
4
```




```output4
32347
```



## Note

<p>In the first example, the only rated string is <span class="tex-font-style-tt">11</span>. So the answer is $1$.</p><p>In the second example, the rated strings are: </p><ul> <li> <span class="tex-font-style-tt">111</span>; </li><li> <span class="tex-font-style-tt">101</span>, because we can perform an operation with $i = 1$ and $j = 3$. </li></ul> So the answer is $2$.<p>In the third sample, the rated strings are: </p><ul> <li> <span class="tex-font-style-tt">1001</span>; </li><li> <span class="tex-font-style-tt">1111</span>; </li><li> <span class="tex-font-style-tt">1011</span>; </li><li> <span class="tex-font-style-tt">1101</span>. </li></ul> So the answer is $4$.
