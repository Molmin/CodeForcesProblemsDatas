## Description

<div><p>Let's introduce some definitions that will be needed later.</p><p>Let $prime(x)$ be the set of prime divisors of $x$. For example, $prime(140) = \{ 2, 5, 7 \}$, $prime(169) = \{ 13 \}$.</p><p>Let $g(x, p)$ be the maximum possible integer $p^k$ where $k$ is an integer such that $x$ is divisible by $p^k$. For example:</p><ul> <li> $g(45, 3) = 9$ ($45$ is divisible by $3^2=9$ but not divisible by $3^3=27$), </li><li> $g(63, 7) = 7$ ($63$ is divisible by $7^1=7$ but not divisible by $7^2=49$). </li></ul><p>Let $f(x, y)$ be the product of $g(y, p)$ for all $p$ in $prime(x)$. For example:</p><ul> <li> $f(30, 70) = g(70, 2) \cdot g(70, 3) \cdot g(70, 5) = 2^1 \cdot 3^0 \cdot 5^1 = 10$, </li><li> $f(525, 63) = g(63, 3) \cdot g(63, 5) \cdot g(63, 7) = 3^2 \cdot 5^0 \cdot 7^1 = 63$. </li></ul><p>You have integers $x$ and $n$. Calculate $f(x, 1) \cdot f(x, 2) \cdot \ldots \cdot f(x, n) \bmod{(10^{9} + 7)}$.</p></div><div class="input-specification"><p>The only line contains integers $x$ and $n$ ($2 \le x \le 10^{9}$, $1 \le n \le 10^{18}$)&nbsp;— the numbers used in formula.</p></div><div class="output-specification"><p>Print the answer.</p></div>

## Input

<p>The only line contains integers $x$ and $n$ ($2 \le x \le 10^{9}$, $1 \le n \le 10^{18}$)&nbsp;— the numbers used in formula.</p>

## Output

<p>Print the answer.</p>





```input1
10 2
```




```input2
20190929 1605
```




```input3
947 987654321987654321
```




```output1
2
```




```output2
363165664
```




```output3
593574252
```



## Note

<p>In the first example, $f(10, 1) = g(1, 2) \cdot g(1, 5) = 1$, $f(10, 2) = g(2, 2) \cdot g(2, 5) = 2$.</p><p>In the second example, actual value of formula is approximately $1.597 \cdot 10^{171}$. Make sure you print the answer modulo $(10^{9} + 7)$.</p><p>In the third example, be careful about overflow issue.</p>
