## Description

<div><p>A number $a_2$ is said to be the arithmetic mean of two numbers $a_1$ and $a_3$, if the following condition holds: $a_1 + a_3 = 2\cdot a_2$. </p><p>We define an arithmetic mean deviation of three numbers $a_1$, $a_2$ and $a_3$ as follows: $d(a_1, a_2, a_3) = |a_1 + a_3 - 2 \cdot a_2|$.</p><p>Arithmetic means a lot to Jeevan. He has three numbers $a_1$, $a_2$ and $a_3$ and he wants to minimize the arithmetic mean deviation $d(a_1, a_2, a_3)$. To do so, he can perform the following operation any number of times (possibly zero):</p><ul> <li> Choose $i, j$ from $\{1, 2, 3\}$ such that $i \ne j$ and increment $a_i$ by $1$ and decrement $a_j$ by $1$ </li></ul><p>Help Jeevan find out the minimum value of $d(a_1, a_2, a_3)$ that can be obtained after applying the operation any number of times.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 5000)$ &nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $a_1$, $a_2$ and $a_3$ $(1 \le a_1, a_2, a_3 \le 10^{8})$.</p></div><div class="output-specification"><p>For each test case, output the minimum value of $d(a_1, a_2, a_3)$ that can be obtained after applying the operation any number of times.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 5000)$ &nbsp;— the number of test cases.</p><p>The first and only line of each test case contains three integers $a_1$, $a_2$ and $a_3$ $(1 \le a_1, a_2, a_3 \le 10^{8})$.</p>

## Output

<p>For each test case, output the minimum value of $d(a_1, a_2, a_3)$ that can be obtained after applying the operation any number of times.</p>





```input1
3
3 4 5
2 2 6
1 6 5
```




```output1
0
1
0
```



## Note

<p>Note that after applying a few operations, the values of $a_1$, $a_2$ and $a_3$ may become negative.</p><p>In the first test case, $4$ is already the Arithmetic Mean of $3$ and $5$.</p><p>$d(3, 4, 5) = |3 + 5 - 2 \cdot 4| = 0$</p><p>In the second test case, we can apply the following operation:</p><p>$(2, 2, 6)$ $\xrightarrow[\text{increment $a_2$}]{\text{decrement $a_1$}}$ $(1, 3, 6)$</p><p>$d(1, 3, 6) = |1 + 6 - 2 \cdot 3| = 1$</p><p>It can be proven that answer can not be improved any further.</p><p>In the third test case, we can apply the following operations:</p><p>$(1, 6, 5)$ $\xrightarrow[\text{increment $a_3$}]{\text{decrement $a_2$}}$ $(1, 5, 6)$ $\xrightarrow[\text{increment $a_1$}]{\text{decrement $a_2$}}$ $(2, 4, 6)$</p><p>$d(2, 4, 6) = |2 + 6 - 2 \cdot 4| = 0$</p>
