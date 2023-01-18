## Description

<div><p>You are given an integer $x$ represented as a product of $n$ its <span class="tex-font-style-it">prime</span> divisors $p_1 \cdot p_2, \cdot \ldots \cdot p_n$. Let $S$ be the set of <span class="tex-font-style-it">all</span> positive integer divisors of $x$ (including $1$ and $x$ itself).</p><p>We call a set of integers $D$ <span class="tex-font-style-it">good</span> if (and only if) there is no pair $a \in D$, $b \in D$ such that $a \ne b$ and $a$ divides $b$.</p><p>Find a <span class="tex-font-style-it">good</span> subset of $S$ with maximum possible size. Since the answer can be large, print the size of the subset modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains the single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of prime divisors in representation of $x$.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($2 \le p_i \le 3 \cdot 10^6$) — the prime factorization of $x$.</p></div><div class="output-specification"><p>Print the maximum possible size of a <span class="tex-font-style-it">good</span> subset modulo $998244353$.</p></div>

## Input

<p>The first line contains the single integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of prime divisors in representation of $x$.</p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($2 \le p_i \le 3 \cdot 10^6$) — the prime factorization of $x$.</p>

## Output

<p>Print the maximum possible size of a <span class="tex-font-style-it">good</span> subset modulo $998244353$.</p>





```input1
3
2999999 43 2999957
```




```input2
6
2 3 2 3 2 2
```




```output1
3
```




```output2
3
```



## Note

<p>In the first sample, $x = 2999999 \cdot 43 \cdot 2999957$ and one of the maximum good subsets is $\{ 43, 2999957, 2999999 \}$.</p><p>In the second sample, $x = 2 \cdot 3 \cdot 2 \cdot 3 \cdot 2 \cdot 2 = 144$ and one of the maximum good subsets is $\{ 9, 12, 16 \}$.</p>
