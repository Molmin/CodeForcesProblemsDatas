## Description

<div><p>Calculate the number of permutations $p$ of size $n$ with exactly $k$ inversions (pairs of indices $(i, j)$ such that $i &lt; j$ and $p_i &gt; p_j$) and exactly $x$ indices $i$ such that $p_i &gt; p_{i+1}$.</p><p>Yep, that's the whole problem. Good luck!</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 3 \cdot 10^4$) — the number of test cases.</p><p>Each test case consists of one line which contains three integers $n$, $k$ and $x$ ($1 \le n \le 998244352$; $1 \le k \le 11$; $1 \le x \le 11$).</p></div><div class="output-specification"><p>For each test case, print one integer — the answer to the problem, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 3 \cdot 10^4$) — the number of test cases.</p><p>Each test case consists of one line which contains three integers $n$, $k$ and $x$ ($1 \le n \le 998244352$; $1 \le k \le 11$; $1 \le x \le 11$).</p>

## Output

<p>For each test case, print one integer — the answer to the problem, taken modulo $998244353$.</p>





```input1
5
10 6 4
7 3 1
163316 11 7
136373 11 1
325902 11 11
```




```output1
465
12
986128624
7636394
57118194
```


