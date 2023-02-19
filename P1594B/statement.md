## Description

<div><p>Theofanis really likes sequences of positive integers, thus his teacher (Yeltsa Kcir) gave him a problem about a sequence that consists of only special numbers.</p><p>Let's call a positive number <span class="tex-font-style-it">special</span> if it can be written as a sum of <span class="tex-font-style-bf">different</span> non-negative powers of $n$. For example, for $n = 4$ number $17$ is special, because it can be written as $4^0 + 4^2 = 1 + 16 = 17$, but $9$ is not.</p><p>Theofanis asks you to help him find the $k$-th special number if they are sorted in increasing order. Since this number may be too large, output it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^9$; $1 \le k \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the $k$-th special number in increasing order modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^9$; $1 \le k \le 10^9$).</p>

## Output

<p>For each test case, print one integer&nbsp;— the $k$-th special number in increasing order modulo $10^9+7$.</p>





```input1
3
3 4
2 12
105 564
```




```output1
9
12
3595374
```



## Note

<p>For $n = 3$ the sequence is $[1,3,4,9...]$</p>
