## Description

<div><p>Let's define a function $f(p)$ on a permutation $p$ as follows. Let $g_i$ be the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of elements $p_1$, $p_2$, ..., $p_i$ (in other words, it is the GCD of the prefix of length $i$). Then $f(p)$ is the number of <span class="tex-font-style-bf">distinct</span> elements among $g_1$, $g_2$, ..., $g_n$.</p><p>Let $f_{max}(n)$ be the maximum value of $f(p)$ among all permutations $p$ of integers $1$, $2$, ..., $n$.</p><p>Given an integers $n$, count the number of permutations $p$ of integers $1$, $2$, ..., $n$, such that $f(p)$ is equal to $f_{max}(n)$. Since the answer may be large, print the remainder of its division by $1000\,000\,007 = 10^9 + 7$.</p></div><div class="input-specification"><p>The only line contains the integer $n$ ($2 \le n \le 10^6$)&nbsp;— the length of the permutations.</p></div><div class="output-specification"><p>The only line should contain your answer modulo $10^9+7$.</p></div>

## Input

<p>The only line contains the integer $n$ ($2 \le n \le 10^6$)&nbsp;— the length of the permutations.</p>

## Output

<p>The only line should contain your answer modulo $10^9+7$.</p>





```input1
2
```




```input2
3
```




```input3
6
```




```output1
1
```




```output2
4
```




```output3
120
```



## Note

<p>Consider the second example: these are the permutations of length $3$:</p><ul> <li> $[1,2,3]$, $f(p)=1$. </li><li> $[1,3,2]$, $f(p)=1$. </li><li> $[2,1,3]$, $f(p)=2$. </li><li> $[2,3,1]$, $f(p)=2$. </li><li> $[3,1,2]$, $f(p)=2$. </li><li> $[3,2,1]$, $f(p)=2$. </li></ul><p>The maximum value $f_{max}(3) = 2$, and there are $4$ permutations $p$ such that $f(p)=2$.</p>
