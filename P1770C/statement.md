## Description

<div><p>Joi has an array $a$ of $n$ <span class="tex-font-style-bf">positive</span> integers. Koxia wants you to determine whether there exists a <span class="tex-font-style-bf">positive</span> integer $x &gt; 0$ such that $\gcd(a_i+x,a_j+x)=1$ for all $1 \leq i &lt; j \leq n$.</p><p>Here $\gcd(y, z)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest&nbsp;common divisor (GCD)</a> of integers $y$ and $z$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 100$) — the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq {10}^{18}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p></div><div class="output-specification"><p>For each test case, output "YES" (without quotes) if there exists a positive integer $x$ such that $\gcd(a_i+x,a_j+x)=1$ for all $1 \leq i &lt; j \leq n$, and "NO" (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "yEs", "yes", "Yes", and "YES" will be recognized as positive responses.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 100$) — the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq {10}^{18}$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$.</p>

## Output

<p>For each test case, output "YES" (without quotes) if there exists a positive integer $x$ such that $\gcd(a_i+x,a_j+x)=1$ for all $1 \leq i &lt; j \leq n$, and "NO" (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "yEs", "yes", "Yes", and "YES" will be recognized as positive responses.</p>





```input1|2,3
2
3
5 7 10
3
3 3 4
```




```output1
YES
NO
```



## Note

<p>In the first test case, we can set $x = 4$. This is valid because: </p><ul> <li> When $i=1$ and $j=2$, $\gcd(a_i+x,a_j+x)=\gcd(5+4,7+4)=\gcd(9,11)=1$. </li><li> When $i=1$ and $j=3$, $\gcd(a_i+x,a_j+x)=\gcd(5+4,10+4)=\gcd(9,14)=1$. </li><li> When $i=2$ and $j=3$, $\gcd(a_i+x,a_j+x)=\gcd(7+4,10+4)=\gcd(11,14)=1$. </li></ul><p>In the second test case, any choice of $x$ makes $\gcd(a_1 + x, a_2 + x) = \gcd(3+x,3+x)=3+x$. Therefore, no such $x$ exists.</p>
