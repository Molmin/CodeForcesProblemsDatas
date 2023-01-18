## Description

<div><p>You are given two integers $A$ and $B$, calculate the number of pairs $(a, b)$ such that $1 \le a \le A$, $1 \le b \le B$, and the equation $a \cdot b + a + b = conc(a, b)$ is true; $conc(a, b)$ is the concatenation of $a$ and $b$ (for example, $conc(12, 23) = 1223$, $conc(100, 11) = 10011$). <span class="tex-font-style-bf">$a$ and $b$ should not contain leading zeroes</span>.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Each test case contains two integers $A$ and $B$ $(1 \le A, B \le 10^9)$.</p></div><div class="output-specification"><p>Print one integer — the number of pairs $(a, b)$ such that $1 \le a \le A$, $1 \le b \le B$, and the equation $a \cdot b + a + b = conc(a, b)$ is true.</p></div>

## Input

<p>The first line contains $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Each test case contains two integers $A$ and $B$ $(1 \le A, B \le 10^9)$.</p>

## Output

<p>Print one integer — the number of pairs $(a, b)$ such that $1 \le a \le A$, $1 \le b \le B$, and the equation $a \cdot b + a + b = conc(a, b)$ is true.</p>





```input1|2,4
3
1 11
4 2
191 31415926
```




```output1
1
0
1337
```



## Note

<p>There is only one suitable pair in the first test case: $a = 1$, $b = 9$ ($1 + 9 + 1 \cdot 9 = 19$).</p>
