## Description

<div><p>You are given a string $t$ consisting of $n$ lowercase Latin letters and an integer number $k$.</p><p>Let's define a substring of some string $s$ with indices from $l$ to $r$ as $s[l \dots r]$.</p><p>Your task is to construct such string $s$ of minimum possible length that there are exactly $k$ positions $i$ such that $s[i \dots i + n - 1] = t$. In other words, your task is to construct such string $s$ of minimum possible length that there are exactly $k$ substrings of $s$ equal to $t$.</p><p>It is guaranteed that the answer is always unique.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n, k \le 50$) — the length of the string $t$ and the number of substrings.</p><p>The second line of the input contains the string $t$ consisting of exactly $n$ lowercase Latin letters.</p></div><div class="output-specification"><p>Print such string $s$ of minimum possible length that there are exactly $k$ substrings of $s$ equal to $t$.</p><p>It is guaranteed that the answer is always unique.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n, k \le 50$) — the length of the string $t$ and the number of substrings.</p><p>The second line of the input contains the string $t$ consisting of exactly $n$ lowercase Latin letters.</p>

## Output

<p>Print such string $s$ of minimum possible length that there are exactly $k$ substrings of $s$ equal to $t$.</p><p>It is guaranteed that the answer is always unique.</p>





```input1
3 4
aba

```




```input2
3 2
cat

```




```output1
ababababa

```




```output2
catcat

```


