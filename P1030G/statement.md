## Description

<div><p>You are given a tuple generator $f^{(k)} = (f_1^{(k)}, f_2^{(k)}, \dots, f_n^{(k)})$, where $f_i^{(k)} = (a_i \cdot f_i^{(k - 1)} + b_i) \bmod p_i$ and $f^{(0)} = (x_1, x_2, \dots, x_n)$. Here $x \bmod y$ denotes the remainder of $x$ when divided by $y$. All $p_i$ are primes.</p><p>One can see that with fixed sequences $x_i$, $y_i$, $a_i$ the tuples $f^{(k)}$ starting from some index will repeat tuples with smaller indices. Calculate the maximum number of different tuples (from all $f^{(k)}$ for $k \ge 0$) that can be produced by this generator, if $x_i$, $a_i$, $b_i$ are integers in the range $[0, p_i - 1]$ and can be chosen arbitrary. The answer can be large, so print the remainder it gives when divided by $10^9 + 7$</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in the tuple.</p><p>The second line contains $n$ space separated prime numbers — the modules $p_1, p_2, \ldots, p_n$ ($2 \le p_i \le 2 \cdot 10^6$).</p></div><div class="output-specification"><p>Print one integer — the maximum number of different tuples modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of elements in the tuple.</p><p>The second line contains $n$ space separated prime numbers — the modules $p_1, p_2, \ldots, p_n$ ($2 \le p_i \le 2 \cdot 10^6$).</p>

## Output

<p>Print one integer — the maximum number of different tuples modulo $10^9 + 7$.</p>





```input1
4
2 3 5 7

```




```input2
3
5 3 3

```




```output1
210

```




```output2
30

```



## Note

<p>In the first example we can choose next parameters: $a = [1, 1, 1, 1]$, $b = [1, 1, 1, 1]$, $x = [0, 0, 0, 0]$, then $f_i^{(k)} = k \bmod p_i$.</p><p>In the second example we can choose next parameters: $a = [1, 1, 2]$, $b = [1, 1, 0]$, $x = [0, 0, 1]$.</p>
