## Description

<div><p>You are given two positive (greater than zero) integers $x$ and $y$. There is a variable $k$ initially set to $0$.</p><p>You can perform the following two types of operations: </p><ul> <li> add $1$ to $k$ (i. e. assign $k := k + 1$); </li><li> add $x \cdot 10^{p}$ to $k$ for some non-negative $p$ (i. e. assign $k := k + x \cdot 10^{p}$ for some $p \ge 0$). </li></ul><p>Find the minimum number of operations described above to set the value of $k$ to $y$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing two integer $x$ and $y$ ($1 \le x, y \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print one integer — the minimum number of operations to set the value of $k$ to $y$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing two integer $x$ and $y$ ($1 \le x, y \le 10^9$).</p>

## Output

<p>For each test case, print one integer — the minimum number of operations to set the value of $k$ to $y$.</p>





```input1
3
2 7
3 42
25 1337
```




```output1
4
5
20
```



## Note

<p>In the first test case you can use the following sequence of operations: </p><ol> <li> add $1$; </li><li> add $2 \cdot 10^0 = 2$; </li><li> add $2 \cdot 10^0 = 2$; </li><li> add $2 \cdot 10^0 = 2$. </li></ol> $1 + 2 + 2 + 2 = 7$.<p>In the second test case you can use the following sequence of operations: </p><ol> <li> add $3 \cdot 10^1 = 30$; </li><li> add $3 \cdot 10^0 = 3$; </li><li> add $3 \cdot 10^0 = 3$; </li><li> add $3 \cdot 10^0 = 3$; </li><li> add $3 \cdot 10^0 = 3$. </li></ol> $30 + 3 + 3 + 3 + 3 = 42$.
