## Description

<div><p>You are given an integer $n$. Find a sequence of $n$ integers $a_1, a_2, \dots, a_n$ such that $1 \leq a_i \leq 10^9$ for all $i$ and $$a_1 \oplus a_2 \oplus \dots \oplus a_n = \frac{a_1 + a_2 + \dots + a_n}{n},$$ where $\oplus$ represents the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a>.</p><p>It can be proven that there exists a sequence of integers that satisfies all the conditions above.</p></div><div class="input-specification"><p>The first line of input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains one integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the length of the sequence you have to find.</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ space-separated integers $a_1, a_2, \dots, a_n$ satisfying the conditions in the statement. </p><p>If there are several possible answers, you can output any of them.</p></div>

## Input

<p>The first line of input contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains one integer $n$ ($1 \leq n \leq 10^5$)&nbsp;— the length of the sequence you have to find.</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output $n$ space-separated integers $a_1, a_2, \dots, a_n$ satisfying the conditions in the statement. </p><p>If there are several possible answers, you can output any of them.</p>





```input1|2,4
3
1
4
3
```




```output1
69
13 2 8 1
7 7 7
```



## Note

<p>In the first test case, $69 = \frac{69}{1} = 69$.</p><p>In the second test case, $13 \oplus 2 \oplus 8 \oplus 1 = \frac{13 + 2 + 8 + 1}{4} = 6$.</p>
