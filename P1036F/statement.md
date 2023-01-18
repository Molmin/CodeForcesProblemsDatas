## Description

<div><p>Consider some positive integer $x$. Its prime factorization will be of form $x = 2^{k_1} \cdot 3^{k_2} \cdot 5^{k_3} \cdot \dots$</p><p>Let's call $x$ <span class="tex-font-style-it">elegant</span> if the greatest common divisor of the sequence $k_1, k_2, \dots$ is equal to $1$. For example, numbers $5 = 5^1$, $12 = 2^2 \cdot 3$, $72 = 2^3 \cdot 3^2$ are <span class="tex-font-style-it">elegant</span> and numbers $8 = 2^3$ ($GCD = 3$), $2500 = 2^2 \cdot 5^4$ ($GCD = 2$) are not.</p><p>Count the number of <span class="tex-font-style-it">elegant</span> integers from $2$ to $n$.</p><p>Each testcase contains several values of $n$, for each of them you are required to solve the problem separately.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 10^5$) — the number of values of $n$ in the testcase.</p><p>Each of the next $T$ lines contains a single integer $n_i$ ($2 \le n_i \le 10^{18}$).</p></div><div class="output-specification"><p>Print $T$ lines — the $i$-th line should contain the number of <span class="tex-font-style-it">elegant</span> numbers from $2$ to $n_i$.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 10^5$) — the number of values of $n$ in the testcase.</p><p>Each of the next $T$ lines contains a single integer $n_i$ ($2 \le n_i \le 10^{18}$).</p>

## Output

<p>Print $T$ lines — the $i$-th line should contain the number of <span class="tex-font-style-it">elegant</span> numbers from $2$ to $n_i$.</p>





```input1
4
4
2
72
10

```




```output1
2
1
61
6

```



## Note

<p>Here is the list of <span class="tex-font-style-bf">non-elegant</span> numbers up to $10$:</p><ul> <li> $4 = 2^2, GCD = 2$; </li><li> $8 = 2^3, GCD = 3$; </li><li> $9 = 3^2, GCD = 2$. </li></ul><p>The rest have $GCD = 1$.</p>
