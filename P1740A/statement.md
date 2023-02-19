## Description

<div><p>Pak Chanek has a prime number$^\dagger$ $n$. Find a prime number $m$ such that $n + m$ is not prime.</p><p>$^\dagger$ A prime number is a number with <span class="tex-font-style-bf">exactly</span> $2$ factors. The first few prime numbers are $2,3,5,7,11,13,\ldots$. In particular, $1$ is <span class="tex-font-style-bf">not</span> a prime number.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The following lines contain the description of each test case.</p><p>The only line of each test case contains a prime number $n$ ($2 \leq n \leq 10^5$).</p></div><div class="output-specification"><p>For each test case, output a line containing a prime number $m$ ($2 \leq m \leq 10^5$) such that $n + m$ is not prime. It can be proven that under the constraints of the problem, such $m$ always exists.</p><p>If there are multiple solutions, you can output any of them. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The following lines contain the description of each test case.</p><p>The only line of each test case contains a prime number $n$ ($2 \leq n \leq 10^5$).</p>

## Output

<p>For each test case, output a line containing a prime number $m$ ($2 \leq m \leq 10^5$) such that $n + m$ is not prime. It can be proven that under the constraints of the problem, such $m$ always exists.</p><p>If there are multiple solutions, you can output any of them. </p>





```input1|2,4
3
7
2
75619
```




```output1
2
7
47837
```



## Note

<p>In the first test case, $m = 2$, which is prime, and $n + m = 7 + 2 = 9$, which is not prime.</p><p>In the second test case, $m = 7$, which is prime, and $n + m = 2 + 7 = 9$, which is not prime.</p><p>In the third test case, $m = 47837$, which is prime, and $n + m = 75619 + 47837 = 123456$, which is not prime.</p>
