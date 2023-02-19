## Description

<div><p>You are given an array $a_1, a_2, \ldots, a_n$ and an integer $x$.</p><p>Find the number of non-empty subsets of indices of this array $1 \leq b_1 &lt; b_2 &lt; \ldots &lt; b_k \leq n$, such that for all pairs $(i, j)$ where $1 \leq i &lt; j \leq k$, the inequality $a_{b_i} \oplus a_{b_j} \leq x$ is held. Here, $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. As the answer may be very large, output it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $x$ ($1 \leq n \leq 150\,000$, $0 \leq x &lt; 2^{30}$). Here, $n$ is the size of the array.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 2^{30}$): the array itself.</p></div><div class="output-specification"><p>Print one integer: the number of non-empty subsets such that the bitwise XOR of every pair of elements is at most $x$, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $x$ ($1 \leq n \leq 150\,000$, $0 \leq x &lt; 2^{30}$). Here, $n$ is the size of the array.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i &lt; 2^{30}$): the array itself.</p>

## Output

<p>Print one integer: the number of non-empty subsets such that the bitwise XOR of every pair of elements is at most $x$, modulo $998\,244\,353$.</p>





```input1
4 2
0 1 2 3
```




```input2
3 6
4 2 2
```




```input3
4 0
1 1 2 2
```




```output1
8
```




```output2
7
```




```output3
6
```


