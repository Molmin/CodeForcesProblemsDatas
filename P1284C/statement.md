## Description

<div><p>Recall that the permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>A sequence $a$ is a subsegment of a sequence $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end. We will denote the subsegments as $[l, r]$, where $l, r$ are two integers with $1 \le l \le r \le n$. This indicates the subsegment where $l-1$ elements from the beginning and $n-r$ elements from the end are deleted from the sequence.</p><p>For a permutation $p_1, p_2, \ldots, p_n$, we define a <span class="tex-font-style-it">framed segment</span> as a subsegment $[l,r]$ where $\max\{p_l, p_{l+1}, \dots, p_r\} - \min\{p_l, p_{l+1}, \dots, p_r\} = r - l$. For example, for the permutation $(6, 7, 1, 8, 5, 3, 2, 4)$ some of its framed segments are: $[1, 2], [5, 8], [6, 7], [3, 3], [8, 8]$. In particular, a subsegment $[i,i]$ is always a framed segments for any $i$ between $1$ and $n$, inclusive.</p><p>We define the <span class="tex-font-style-it">happiness</span> of a permutation $p$ as the number of pairs $(l, r)$ such that $1 \le l \le r \le n$, and $[l, r]$ is a framed segment. For example, the permutation $[3, 1, 2]$ has happiness $5$: all segments except $[1, 2]$ are framed segments.</p><p>Given integers $n$ and $m$, Jongwon wants to compute the sum of happiness for all permutations of length $n$, modulo the prime number $m$. Note that there exist $n!$ (factorial of $n$) different permutations of length $n$.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $m$ ($1 \le n \le 250\,000$, $10^8 \le m \le 10^9$, $m$ is prime).</p></div><div class="output-specification"><p>Print $r$ ($0 \le r &lt; m$), the sum of happiness for all permutations of length $n$, modulo a prime number $m$.</p></div>

## Input

<p>The only line contains two integers $n$ and $m$ ($1 \le n \le 250\,000$, $10^8 \le m \le 10^9$, $m$ is prime).</p>

## Output

<p>Print $r$ ($0 \le r &lt; m$), the sum of happiness for all permutations of length $n$, modulo a prime number $m$.</p>





```input1
1 993244853
```




```input2
2 993244853
```




```input3
3 993244853
```




```input4
2019 993244853
```




```input5
2020 437122297
```




```output1
1
```




```output2
6
```




```output3
32
```




```output4
923958830
```




```output5
265955509
```



## Note

<p>For sample input $n=3$, let's consider all permutations of length $3$:</p><ul> <li> $[1, 2, 3]$, all subsegments are framed segment. Happiness is $6$. </li><li> $[1, 3, 2]$, all subsegments except $[1, 2]$ are framed segment. Happiness is $5$. </li><li> $[2, 1, 3]$, all subsegments except $[2, 3]$ are framed segment. Happiness is $5$. </li><li> $[2, 3, 1]$, all subsegments except $[2, 3]$ are framed segment. Happiness is $5$. </li><li> $[3, 1, 2]$, all subsegments except $[1, 2]$ are framed segment. Happiness is $5$. </li><li> $[3, 2, 1]$, all subsegments are framed segment. Happiness is $6$. </li></ul><p>Thus, the sum of happiness is $6+5+5+5+5+6 = 32$.</p>
