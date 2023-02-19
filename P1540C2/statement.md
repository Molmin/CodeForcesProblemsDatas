## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is that in this version $1 \le q \le 10^5$. You can make hacks only if both versions of the problem are solved.</span></p><p>There is a process that takes place on arrays $a$ and $b$ of length $n$ and length $n-1$ respectively. </p><p>The process is an infinite sequence of operations. Each operation is as follows: </p><ul> <li> First, choose a random integer $i$ ($1 \le i \le n-1$). </li><li> Then, simultaneously set $a_i = \min\left(a_i, \frac{a_i+a_{i+1}-b_i}{2}\right)$ and $a_{i+1} = \max\left(a_{i+1}, \frac{a_i+a_{i+1}+b_i}{2}\right)$ without any rounding (so values may become non-integer). </li></ul> See notes for an example of an operation.<p>It can be proven that array $a$ converges, i.&nbsp;e. for each $i$ there exists a limit $a_i$ converges to. Let function $F(a, b)$ return the value $a_1$ converges to after a process on $a$ and $b$.</p><p>You are given array $b$, but not array $a$. However, you are given a third array $c$. Array $a$ is good if it contains only <span class="tex-font-style-bf">integers</span> and satisfies $0 \leq a_i \leq c_i$ for $1 \leq i \leq n$.</p><p>Your task is to count the number of good arrays $a$ where $F(a, b) \geq x$ for $q$ values of $x$. Since the number of arrays can be very large, print it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 100$).</p><p>The second line contains $n$ integers $c_1, c_2 \ldots, c_n$ ($0 \le c_i \le 100$).</p><p>The third line contains $n-1$ integers $b_1, b_2, \ldots, b_{n-1}$ ($0 \le b_i \le 100$).</p><p>The fourth line contains a single integer $q$ ($1 \le q \le 10^5$).</p><p>The fifth line contains $q$ space separated integers $x_1, x_2, \ldots, x_q$ ($-10^5 \le x_i \le 10^5$).</p></div><div class="output-specification"><p>Output $q$ integers, where the $i$-th integer is the answer to the $i$-th query, i.&nbsp;e. the number of good arrays $a$ where $F(a, b) \geq x_i$ modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 100$).</p><p>The second line contains $n$ integers $c_1, c_2 \ldots, c_n$ ($0 \le c_i \le 100$).</p><p>The third line contains $n-1$ integers $b_1, b_2, \ldots, b_{n-1}$ ($0 \le b_i \le 100$).</p><p>The fourth line contains a single integer $q$ ($1 \le q \le 10^5$).</p><p>The fifth line contains $q$ space separated integers $x_1, x_2, \ldots, x_q$ ($-10^5 \le x_i \le 10^5$).</p>

## Output

<p>Output $q$ integers, where the $i$-th integer is the answer to the $i$-th query, i.&nbsp;e. the number of good arrays $a$ where $F(a, b) \geq x_i$ modulo $10^9+7$.</p>





```input1
3
2 3 4
2 1
5
-1 0 1 -100000 100000
```




```output1
56
28
4
60
0
```



## Note

<p>The following explanation assumes $b = [2, 1]$ and $c=[2, 3, 4]$ (as in the sample).</p><p>Examples of arrays $a$ that are <span class="tex-font-style-bf">not</span> good: </p><ul> <li> $a = [3, 2, 3]$ is not good because $a_1 &gt; c_1$; </li><li> $a = [0, -1, 3]$ is not good because $a_2 &lt; 0$. </li></ul><p>One possible good array $a$ is $[0, 2, 4]$. We can show that no operation has any effect on this array, so $F(a, b) = a_1 = 0$.</p><p>Another possible good array $a$ is $[0, 1, 4]$. In a single operation with $i = 1$, we set $a_1 = \min(\frac{0+1-2}{2}, 0)$ and $a_2 = \max(\frac{0+1+2}{2}, 1)$. So, after a single operation with $i = 1$, $a$ becomes equal to $[-\frac{1}{2}, \frac{3}{2}, 4]$. We can show that no operation has any effect on this array, so $F(a, b) = -\frac{1}{2}$.</p>
