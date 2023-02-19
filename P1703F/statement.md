## Description

<div><p>You are given an array $a_1, a_2, \dots a_n$. Count the number of pairs of indices $1 \leq i, j \leq n$ such that $a_i &lt; i &lt; a_j &lt; j$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of pairs of indices satisfying the condition in the statement.</p><p>Please note, that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2 \cdot 10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of pairs of indices satisfying the condition in the statement.</p><p>Please note, that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p>





```input1|2,3,6,7,10,11
5
8
1 1 2 3 8 2 1 4
2
1 2
10
0 2 1 6 3 4 1 2 8 3
2
1 1000000000
3
0 1000000000 2
```




```output1
3
0
10
0
1
```



## Note

<p>For the first test cases the pairs are $(i, j)$ = $\{(2, 4), (2, 8), (3, 8)\}$. </p><ul> <li> The pair $(2, 4)$ is true because $a_2 = 1$, $a_4 = 3$ and $1 &lt; 2 &lt; 3 &lt; 4$. </li><li> The pair $(2, 8)$ is true because $a_2 = 1$, $a_8 = 4$ and $1 &lt; 2 &lt; 4 &lt; 8$. </li><li> The pair $(3, 8)$ is true because $a_3 = 2$, $a_8 = 4$ and $2 &lt; 3 &lt; 4 &lt; 8$. </li></ul>
