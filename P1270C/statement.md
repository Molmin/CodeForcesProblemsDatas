## Description

<div><p>Let's call an array $a_1, a_2, \dots, a_m$ of nonnegative integer numbers <span class="tex-font-style-bf">good</span> if $a_1 + a_2 + \dots + a_m = 2\cdot(a_1 \oplus a_2 \oplus \dots \oplus a_m)$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>For example, array $[1, 2, 3, 6]$ is good, as $1 + 2 + 3 + 6 = 12 = 2\cdot 6 = 2\cdot (1\oplus 2 \oplus 3 \oplus 6)$. At the same time, array $[1, 2, 1, 3]$ isn't good, as $1 + 2 + 1 + 3 = 7 \neq 2\cdot 1 = 2\cdot(1\oplus 2 \oplus 1 \oplus 3)$.</p><p>You are given an array of length $n$: $a_1, a_2, \dots, a_n$. Append at most $3$ elements to it to make it good. Appended elements don't have to be different. It can be shown that the solution always exists under the given constraints. If there are different solutions, you are allowed to output any of them. Note that <span class="tex-font-style-bf">you don't have to minimize the number of added elements!</span>. So, if an array is good already you are allowed to not append elements.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1\le n \le 10^5)$&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0\le a_i \le 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output two lines.</p><p>In the first line, output a single integer $s$ ($0\le s\le 3$)&nbsp;— the number of elements you want to append.</p><p>In the second line, output $s$ integers $b_1, \dots, b_s$ ($0\le b_i \le 10^{18}$)&nbsp;— the elements you want to append to the array.</p><p>If there are different solutions, you are allowed to output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1\le n \le 10^5)$&nbsp;— the size of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($0\le a_i \le 10^9$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output two lines.</p><p>In the first line, output a single integer $s$ ($0\le s\le 3$)&nbsp;— the number of elements you want to append.</p><p>In the second line, output $s$ integers $b_1, \dots, b_s$ ($0\le b_i \le 10^{18}$)&nbsp;— the elements you want to append to the array.</p><p>If there are different solutions, you are allowed to output any of them.</p>





```input1
3
4
1 2 3 6
1
8
2
1 1
```




```output1
0

2
4 4
3
2 6 2
```



## Note

<p>In the first test case of the example, the sum of all numbers is $12$, and their $\oplus$ is $6$, so the condition is already satisfied.</p><p>In the second test case of the example, after adding $4, 4$, the array becomes $[8, 4, 4]$. The sum of numbers in it is $16$, $\oplus$ of numbers in it is $8$.</p>
