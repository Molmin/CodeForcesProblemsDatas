## Description

<div><p>There is a chip on the coordinate line. Initially, the chip is located at the point $0$. You can perform any number of moves; each move increases the coordinate of the chip by some positive integer (which is called <span class="tex-font-style-it">the length of the move</span>). The length of the first move you make should be divisible by $k$, the length of the second move&nbsp;— by $k+1$, the third&nbsp;— by $k+2$, and so on.</p><p>For example, if $k=2$, then the sequence of moves may look like this: $0 \rightarrow 4 \rightarrow 7 \rightarrow 19 \rightarrow 44$, because $4 - 0 = 4$ is divisible by $2 = k$, $7 - 4 = 3$ is divisible by $3 = k + 1$, $19 - 7 = 12$ is divisible by $4 = k + 2$, $44 - 19 = 25$ is divisible by $5 = k + 3$.</p><p>You are given two positive integers $n$ and $k$. Your task is to count the number of ways to reach the point $x$, starting from $0$, for every $x \in [1, n]$. The number of ways can be very large, so print it modulo $998244353$. Two ways are considered different if they differ as sets of visited positions.</p></div><div class="input-specification"><p>The first (and only) line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>Print $n$ integers&nbsp;— the number of ways to reach the point $x$, starting from $0$, for every $x \in [1, n]$, taken modulo $998244353$.</p></div>

## Input

<p>The first (and only) line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$).</p>

## Output

<p>Print $n$ integers&nbsp;— the number of ways to reach the point $x$, starting from $0$, for every $x \in [1, n]$, taken modulo $998244353$.</p>





```input1
8 1
```




```input2
10 2
```




```output1
1 1 2 2 3 4 5 6
```




```output2
0 1 0 1 1 1 1 2 2 2
```



## Note

<p>Let's look at the first example:</p><p>Ways to reach the point $1$: $[0, 1]$;</p><p>Ways to reach the point $2$: $[0, 2]$;</p><p>Ways to reach the point $3$: $[0, 1, 3]$, $[0, 3]$;</p><p>Ways to reach the point $4$: $[0, 2, 4]$, $[0, 4]$;</p><p>Ways to reach the point $5$: $[0, 1, 5]$, $[0, 3, 5]$, $[0, 5]$;</p><p>Ways to reach the point $6$: $[0, 1, 3, 6]$, $[0, 2, 6]$, $[0, 4, 6]$, $[0, 6]$;</p><p>Ways to reach the point $7$: $[0, 2, 4, 7]$, $[0, 1, 7]$, $[0, 3, 7]$, $[0, 5, 7]$, $[0, 7]$;</p><p>Ways to reach the point $8$: $[0, 3, 5, 8]$, $[0, 1, 5, 8]$, $[0, 2, 8]$, $[0, 4, 8]$, $[0, 6, 8]$, $[0, 8]$.</p>
