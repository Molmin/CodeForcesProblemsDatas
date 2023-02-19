## Description

<div><p>You are given a positive integer $n$. Let's call some positive integer $a$ without leading zeroes palindromic if it remains the same after reversing the order of its digits. Find the number of distinct ways to express $n$ as a sum of positive palindromic integers. Two ways are considered different if the frequency of at least one palindromic integer is different in them. For example, $5=4+1$ and $5=3+1+1$ are considered different but $5=3+1+1$ and $5=1+3+1$ are considered the same. </p><p>Formally, you need to find the number of distinct multisets of positive palindromic integers the sum of which is equal to $n$.</p><p>Since the answer can be quite large, print it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1\leq t\leq 10^4$) denoting the number of testcases.</p><p>Each testcase contains a single line of input containing a single integer $n$ ($1\leq n\leq 4\cdot 10^4$)&nbsp;— the required sum of palindromic integers.</p></div><div class="output-specification"><p>For each testcase, print a single integer denoting the required answer modulo $10^9+7$.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1\leq t\leq 10^4$) denoting the number of testcases.</p><p>Each testcase contains a single line of input containing a single integer $n$ ($1\leq n\leq 4\cdot 10^4$)&nbsp;— the required sum of palindromic integers.</p>

## Output

<p>For each testcase, print a single integer denoting the required answer modulo $10^9+7$.</p>





```input1
2
5
12
```




```output1
7
74
```



## Note

<p>For the first testcase, there are $7$ ways to partition $5$ as a sum of positive palindromic integers: </p><ul> <li> $5=1+1+1+1+1$ </li><li> $5=1+1+1+2$ </li><li> $5=1+2+2$ </li><li> $5=1+1+3$ </li><li> $5=2+3$ </li><li> $5=1+4$ </li><li> $5=5$ </li></ul><p>For the second testcase, there are total $77$ ways to partition $12$ as a sum of positive integers but among them, the partitions $12=2+10$, $12=1+1+10$ and $12=12$ are not valid partitions of $12$ as a sum of positive palindromic integers because $10$ and $12$ are not palindromic. So, there are $74$ ways to partition $12$ as a sum of positive palindromic integers.</p>
