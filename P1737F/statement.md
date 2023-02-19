## Description

<div><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left"><img class="tex-graphics" src="file://Oqy7Ssn0.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-left"><span class="tex-font-style-it">After a long, tough, but fruitful day at DTL, Ela goes home happily. She entertains herself by solving Competitive Programming problems. She prefers short statements, because she already read too many long papers and documentation at work. The problem of the day reads:</span></td></tr></tbody></table><p></p><p>You are given an integer $c$. Suppose that $c$ has $n$ divisors. You have to find a sequence with $n - 1$ integers $[a_1, a_2, ... a_{n - 1}]$, which satisfies the following conditions:</p><ul> <li> Each element is strictly greater than $1$. </li><li> Each element is a divisor of $c$. </li><li> All elements are distinct. </li><li> For all $1 \le i &lt; n - 1$, $\gcd(a_i, a_{i + 1})$ is a prime number. </li></ul><p>In this problem, because $c$ can be too big, the result of prime factorization of $c$ is given instead. Note that $\gcd(x, y)$ denotes the greatest common divisor (GCD) of integers $x$ and $y$ and a prime number is a positive integer which has exactly $2$ divisors.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) - the number of test cases.</p><p>The first line of each test case contains one integer $m$ ($1 \le m \le 16$) - the number of prime factor of $c$.</p><p>The second line of each test case contains $m$ integers $b_1, b_2, \ldots, b_m$ ($1 \le b_i &lt; 2^{20}$) — exponents of corresponding prime factors of $c$, so that $c = p_1^{b_1} \cdot p_2^{b_2} \cdot \ldots \cdot p_m^{b_m}$ and $n = (b_1 + 1)(b_2 + 1) \ldots (b_m + 1)$ hold. $p_i$ is the $i$-th smallest prime number.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $2^{20}$.</p></div><div class="output-specification"><p>Print the answer for each test case, one per line. If there is no sequence for the given $c$, print $-1$.</p><p>Otherwise, print $n - 1$ lines. In $i$-th line, print $m$ space-separated integers. The $j$-th integer of $i$-th line is equal to the exponent of $j$-th prime number from $a_i$.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) - the number of test cases.</p><p>The first line of each test case contains one integer $m$ ($1 \le m \le 16$) - the number of prime factor of $c$.</p><p>The second line of each test case contains $m$ integers $b_1, b_2, \ldots, b_m$ ($1 \le b_i &lt; 2^{20}$) — exponents of corresponding prime factors of $c$, so that $c = p_1^{b_1} \cdot p_2^{b_2} \cdot \ldots \cdot p_m^{b_m}$ and $n = (b_1 + 1)(b_2 + 1) \ldots (b_m + 1)$ hold. $p_i$ is the $i$-th smallest prime number.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $2^{20}$.</p>

## Output

<p>Print the answer for each test case, one per line. If there is no sequence for the given $c$, print $-1$.</p><p>Otherwise, print $n - 1$ lines. In $i$-th line, print $m$ space-separated integers. The $j$-th integer of $i$-th line is equal to the exponent of $j$-th prime number from $a_i$.</p><p>If there are multiple answers, print any of them.</p>





```input1|2,3,6,7,10,11
5
2
1 1
1
1
3
1 1 1
1
4
2
2 1
```




```output1
0 1 
1 1 
1 0 
1 
0 1 1 
0 0 1 
1 0 1 
1 1 0 
0 1 0 
1 1 1 
1 0 0 
-1
2 0 
1 1 
0 1 
2 1 
1 0
```



## Note

<p>In each test case, the values of $c$ are $6$, $2$, $30$, $16$, and $12$ in that order.</p><p>In the first test case, $1$, $2$, $3$, $6$ are divisors of $6$. Here, sequences $[2, 6, 3]$ and $[3, 6, 2]$ can be answer. Permutation $[3, 2, 6]$ is invalid because $\gcd(a_1, a_2) = 1$ is not a prime number.</p><p>In the forth test case, $1$, $2$, $4$, $8$, $16$ are divisors of $16$. Among the permutation of sequence $[2, 4, 8, 16]$, no valid answer exist.</p>
