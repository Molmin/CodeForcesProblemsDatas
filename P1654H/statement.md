## Description

<div><p>Given a list of distinct values, we denote with <span class="tex-font-style-it">first minimum</span>, <span class="tex-font-style-it">second minimum</span>, and <span class="tex-font-style-it">third minimum</span> the three smallest values (in increasing order).</p><p>A permutation $p_1, p_2, \dots, p_n$ is <span class="tex-font-style-it">good</span> if the following statement holds for all pairs $(l,r)$ with $1\le l &lt; l+2 \le r\le n$. </p><ul> <li> If $\{p_l, p_r\}$ are (not necessarily in this order) the first and second minimum of $p_l, p_{l+1}, \dots, p_r$ then the third minimum of $p_l, p_{l+1},\dots, p_r$ is either $p_{l+1}$ or $p_{r-1}$. </li></ul><p>You are given an integer $n$ and a string $s$ of length $m$ consisting of characters "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>".</p><p>Count the number of <span class="tex-font-style-it">good</span> permutations $p_1, p_2,\dots, p_n$ such that, for all $1\le i\le m$, </p><ul> <li> $p_i &lt; p_{i+1}$ if $s_i =$ "<span class="tex-font-style-tt">&lt;</span>"; </li><li> $p_i &gt; p_{i+1}$ if $s_i =$ "<span class="tex-font-style-tt">&gt;</span>". </li></ul> As the result can be very large, you should print it modulo $998\,244\,353$.</div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \leq m \leq \min(100, n-1)$).</p><p>The second line contains a string $s$ of length $m$, consisting of characters "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>".</p></div><div class="output-specification"><p>Print a single integer: the number of good permutations satisfying the constraints described in the statement, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \leq m \leq \min(100, n-1)$).</p><p>The second line contains a string $s$ of length $m$, consisting of characters "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>".</p>

## Output

<p>Print a single integer: the number of good permutations satisfying the constraints described in the statement, modulo $998\,244\,353$.</p>





```input1
5 3
&gt;&gt;&gt;
```




```input2
5 1
&lt;
```




```input3
6 5
&lt;&lt;&gt;&lt;&gt;
```




```input4
10 5
&gt;&lt;&lt;&gt;&lt;
```




```input5
1008 20
&lt;&gt;&lt;&lt;&gt;&gt;&gt;&lt;&lt;&lt;&lt;&lt;&gt;&gt;&gt;&gt;&gt;&gt;&gt;&gt;
```




```output1
5
```




```output2
56
```




```output3
23
```




```output4
83154
```




```output5
284142857
```



## Note

<p>In the first test, there are $5$ good permutations satisfying the constraints given by the string $s$: $[4, 3, 2, 1, 5]$, $[5, 3, 2, 1, 4]$, $[5, 4, 2, 1, 3]$, $[5, 4, 3, 1, 2]$, $[5, 4, 3, 2, 1]$. Each of them </p><ul> <li> is good; </li><li> satisfies $p_1 &gt; p_2$; </li><li> satisfies $p_2 &gt; p_3$; </li><li> satisfies $p_3 &gt; p_4$. </li></ul><p>In the second test, there are $60$ permutations such that $p_1 &lt; p_2$. Only $56$ of them are good: the permutations $[1, 4, 3, 5, 2]$, $[1, 5, 3, 4, 2]$, $[2, 4, 3, 5, 1]$, $[2, 5, 3, 4, 1]$ are not good because the required condition doesn't hold for $(l, r)$ = $(1, 5)$. For example, for the permutation $[2, 4, 3, 5, 1]$, </p><ul> <li> the first minimum and the second minimum are $p_5$ and $p_1$, respectively (so they are $\{p_l, p_r\}$ up to reordering); </li><li> the third minimum is $p_3$ (neither $p_{l+1}$ nor $p_{r-1}$). </li></ul><p>In the third test, there are $23$ good permutations satisfying the constraints given by the string $s$: $[1, 2, 4, 3, 6, 5]$, $[1, 2, 5, 3, 6, 4]$, $[1, 2, 6, 3, 5, 4]$, $[1, 3, 4, 2, 6, 5]$, $[1, 3, 5, 2, 6, 4]$, $[1, 3, 6, 2, 5, 4]$, $[1, 4, 5, 2, 6, 3]$, $[1, 4, 6, 2, 5, 3]$, $[1, 5, 6, 2, 4, 3]$, $[2, 3, 4, 1, 6, 5]$, $[2, 3, 5, 1, 6, 4]$, $[2, 3, 6, 1, 5, 4]$, $[2, 4, 5, 1, 6, 3]$, $[2, 4, 6, 1, 5, 3]$, $[2, 5, 6, 1, 4, 3]$, $[3, 4, 5, 1, 6, 2]$, $[3, 4, 5, 2, 6, 1]$, $[3, 4, 6, 1, 5, 2]$, $[3, 4, 6, 2, 5, 1]$, $[3, 5, 6, 1, 4, 2]$, $[3, 5, 6, 2, 4, 1]$, $[4, 5, 6, 1, 3, 2]$, $[4, 5, 6, 2, 3, 1]$.</p>
