## Description

<div><p>A sequence of non-negative integers $a_1, a_2, \dots, a_n$ is called <span class="tex-font-style-it">growing</span> if for all $i$ from $1$ to $n - 1$ all ones (of binary representation) in $a_i$ are in the places of ones (of binary representation) in $a_{i + 1}$ (in other words, $a_i \:\&amp;\: a_{i + 1} = a_i$, where $\&amp;$ denotes <a href="http://tiny.cc/xpy9uz">bitwise AND</a>). If $n = 1$ then the sequence is considered <span class="tex-font-style-it">growing</span> as well.</p><p>For example, the following four sequences are growing: </p><ul> <li> $[2, 3, 15, 175]$ — in binary it's $[10_2, 11_2, 1111_2, 10101111_2]$; </li><li> $[5]$ — in binary it's $[101_2]$; </li><li> $[1, 3, 7, 15]$ — in binary it's $[1_2, 11_2, 111_2, 1111_2]$; </li><li> $[0, 0, 0]$ — in binary it's $[0_2, 0_2, 0_2]$. </li></ul><p>The following three sequences are non-growing: </p><ul> <li> $[3, 4, 5]$ — in binary it's $[11_2, 100_2, 101_2]$; </li><li> $[5, 4, 3]$ — in binary it's $[101_2, 100_2, 011_2]$; </li><li> $[1, 2, 4, 8]$ — in binary it's $[0001_2, 0010_2, 0100_2, 1000_2]$. </li></ul><p>Consider two sequences of non-negative integers $x_1, x_2, \dots, x_n$ and $y_1, y_2, \dots, y_n$. Let's call this pair of sequences <span class="tex-font-style-it">co-growing</span> if the sequence $x_1 \oplus y_1, x_2 \oplus y_2, \dots, x_n \oplus y_n$ is <span class="tex-font-style-it">growing</span> where $\oplus$ denotes <a href="http://tiny.cc/bry9uz">bitwise XOR</a>.</p><p>You are given a sequence of integers $x_1, x_2, \dots, x_n$. Find the lexicographically minimal sequence $y_1, y_2, \dots, y_n$ such that sequences $x_i$ and $y_i$ are co-growing.</p><p>The sequence $a_1, a_2, \dots, a_n$ is lexicographically smaller than the sequence $b_1, b_2, \dots, b_n$ if there exists $1 \le k \le n$ such that $a_i = b_i$ for any $1 \le i &lt; k$ but $a_k &lt; b_k$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$) — length of the sequence $x_i$.</p><p>The second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($0 \le x_i &lt; 2^{30}$) — elements of the sequence $x_i$.</p><p>It is guaranteed that the sum of $n$ overall all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $n$ integers $y_1, y_2, \dots, y_n$ ($0 \le y_i &lt; 2^{30}$) — lexicographically minimal sequence such that such that it's co-growing with given sequence $x_i$.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$). Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$) — length of the sequence $x_i$.</p><p>The second line contains $n$ integers $x_1, x_2, \dots, x_n$ ($0 \le x_i &lt; 2^{30}$) — elements of the sequence $x_i$.</p><p>It is guaranteed that the sum of $n$ overall all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $n$ integers $y_1, y_2, \dots, y_n$ ($0 \le y_i &lt; 2^{30}$) — lexicographically minimal sequence such that such that it's co-growing with given sequence $x_i$.</p>





```input1
5
4
1 3 7 15
4
1 2 4 8
5
1 2 3 4 5
4
11 13 15 1
1
0
```




```output1
0 0 0 0 
0 1 3 7 
0 1 0 3 2 
0 2 0 14 
0
```


