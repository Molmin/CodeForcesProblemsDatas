## Description

<div><p>Let's call beauty of an array $b_1, b_2, \ldots, b_n$ ($n &gt; 1$) &nbsp;— $\min\limits_{1 \leq i &lt; j \leq n} |b_i - b_j|$.</p><p>You're given an array $a_1, a_2, \ldots a_n$ and a number $k$. Calculate the sum of beauty over all subsequences of the array of length exactly $k$. As this number can be very large, output it modulo $998244353$.</p><p>A sequence $a$ is a subsequence of an array $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements.</p></div><div class="input-specification"><p>The first line contains integers $n, k$ ($2 \le k \le n \le 1000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^5$).</p></div><div class="output-specification"><p>Output one integer&nbsp;— the sum of beauty over all subsequences of the array of length exactly $k$. As this number can be very large, output it modulo $998244353$.</p></div>

## Input

<p>The first line contains integers $n, k$ ($2 \le k \le n \le 1000$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^5$).</p>

## Output

<p>Output one integer&nbsp;— the sum of beauty over all subsequences of the array of length exactly $k$. As this number can be very large, output it modulo $998244353$.</p>





```input1
4 3
1 7 3 5
```




```input2
5 5
1 10 100 1000 10000
```




```output1
8
```




```output2
9
```



## Note

<p>In the first example, there are $4$ subsequences of length $3$&nbsp;— $[1, 7, 3]$, $[1, 3, 5]$, $[7, 3, 5]$, $[1, 7, 5]$, each of which has beauty $2$, so answer is $8$.</p><p>In the second example, there is only one subsequence of length $5$&nbsp;— the whole array, which has the beauty equal to $|10-1| = 9$.</p>
