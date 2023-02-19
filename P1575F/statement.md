## Description

<div><p>Mr. Chanek opened a letter from his fellow, who is currently studying at Singanesia. Here is what it says.</p><p>Define an array $b$ ($0 \leq b_i &lt; k$) with $n$ integers. While there exists a pair $(i, j)$ such that $b_i \ne b_j$, do the following operation:</p><ul> <li> Randomly pick a number $i$ satisfying $0 \leq i &lt; n$. Note that each number $i$ has a probability of $\frac{1}{n}$ to be picked. </li><li> Randomly Pick a number $j$ satisfying $0 \leq j &lt; k$. </li><li> Change the value of $b_i$ to $j$. It is possible for $b_i$ to be changed to the same value. </li></ul><p>Denote $f(b)$ as the expected number of operations done to $b$ until all elements of $b$ are equal. </p><p>You are given two integers $n$ and $k$, and an array $a$ ($-1 \leq a_i &lt; k$) of $n$ integers. </p><p>For every index $i$ with $a_i = -1$, replace $a_i$ with a random number $j$ satisfying $0 \leq j &lt; k$. Let $c$ be the number of occurrences of $-1$ in $a$. There are $k^c$ possibilites of $a$ after the replacement, each with equal probability of being the final array.</p><p>Find the expected value of $f(a)$ modulo $10^9 + 7$. </p><p>Formally, let $M = 10^9 + 7$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p><p>After reading the letter, Mr. Chanek gave the task to you. Solve it for the sake of their friendship!</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \leq n \leq 10^5$, $2 \leq k \leq 10^9$). </p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-1 \leq a_i &lt; k$).</p></div><div class="output-specification"><p>Output an integer denoting the expected value of $f(a)$ modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \leq n \leq 10^5$, $2 \leq k \leq 10^9$). </p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-1 \leq a_i &lt; k$).</p>

## Output

<p>Output an integer denoting the expected value of $f(a)$ modulo $10^9 + 7$.</p>





```input1
2 2
0 1
```




```input2
2 2
0 -1
```




```input3
3 3
0 1 1
```




```input4
3 3
-1 -1 -1
```




```input5
10 9
-1 0 -1 1 1 2 2 3 3 3
```




```output1
2
```




```output2
1
```




```output3
12
```




```output4
11
```




```output5
652419213
```


