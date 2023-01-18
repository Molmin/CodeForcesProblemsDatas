## Description

<div><p>Can the greatest common divisor and bitwise operations have anything in common? It is time to answer this question.</p><p>Suppose you are given a positive integer $a$. You want to choose some integer $b$ from $1$ to $a - 1$ inclusive in such a way that the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $a \oplus b$ and $a \&gt; \&amp; \&gt; b$ is as large as possible. In other words, you'd like to compute the following function:</p><p>$$f(a) = \max_{0 &lt; b &lt; a}{gcd(a \oplus b, a \&gt; \&amp; \&gt; b)}.$$</p><p>Here $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>, and $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>.</p><p>The greatest common divisor of two integers $x$ and $y$ is the largest integer $g$ such that both $x$ and $y$ are divided by $g$ without remainder.</p><p>You are given $q$ integers $a_1, a_2, \ldots, a_q$. For each of these integers compute the largest possible value of the greatest common divisor (when $b$ is chosen optimally). </p></div><div class="input-specification"><p>The first line contains an integer $q$ ($1 \le q \le 10^3$)&nbsp;— the number of integers you need to compute the answer for.</p><p>After that $q$ integers are given, one per line: $a_1, a_2, \ldots, a_q$ ($2 \le a_i \le 2^{25} - 1$)&nbsp;— the integers you need to compute the answer for. </p></div><div class="output-specification"><p>For each integer, print the answer in the same order as the integers are given in input.</p></div>

## Input

<p>The first line contains an integer $q$ ($1 \le q \le 10^3$)&nbsp;— the number of integers you need to compute the answer for.</p><p>After that $q$ integers are given, one per line: $a_1, a_2, \ldots, a_q$ ($2 \le a_i \le 2^{25} - 1$)&nbsp;— the integers you need to compute the answer for. </p>

## Output

<p>For each integer, print the answer in the same order as the integers are given in input.</p>





```input1
3
2
3
5
```




```output1
3
1
7
```



## Note

<p>For the first integer the optimal choice is $b = 1$, then $a \oplus b = 3$, $a \&gt; \&amp; \&gt; b = 0$, and the greatest common divisor of $3$ and $0$ is $3$.</p><p>For the second integer one optimal choice is $b = 2$, then $a \oplus b = 1$, $a \&gt; \&amp; \&gt; b = 2$, and the greatest common divisor of $1$ and $2$ is $1$.</p><p>For the third integer the optimal choice is $b = 2$, then $a \oplus b = 7$, $a \&gt; \&amp; \&gt; b = 0$, and the greatest common divisor of $7$ and $0$ is $7$.</p>
