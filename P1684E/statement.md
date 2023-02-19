## Description

<div><p>You are given an array $a$ of $n$ non-negative integers. In one operation you can change any number in the array to any other non-negative integer.</p><p>Let's define the <span class="tex-font-style-it">cost</span> of the array as $\operatorname{DIFF}(a) - \operatorname{MEX}(a)$, where $\operatorname{MEX}$ of a set of non-negative integers is the smallest non-negative integer not present in the set, and $\operatorname{DIFF}$ is the number of different numbers in the array.</p><p>For example, $\operatorname{MEX}(\{1, 2, 3\}) = 0$, $\operatorname{MEX}(\{0, 1, 2, 4, 5\}) = 3$.</p><p>You should find the minimal cost of the array $a$ if you are allowed to make at most $k$ operations.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $0 \le k \le 10^5$)&nbsp;— the length of the array $a$ and the number of operations that you are allowed to make.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer&nbsp;— minimal cost that it is possible to get making at most $k$ operations.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $0 \le k \le 10^5$)&nbsp;— the length of the array $a$ and the number of operations that you are allowed to make.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output a single integer&nbsp;— minimal cost that it is possible to get making at most $k$ operations.</p>





```input1|2,3,6,7
4
4 1
3 0 1 2
4 1
0 2 4 5
7 2
4 13 0 0 13 1337 1000000000
6 2
1 2 8 0 0 0
```




```output1
0
1
2
0
```



## Note

<p>In the first test case no operations are needed to minimize the value of $\operatorname{DIFF} - \operatorname{MEX}$.</p><p>In the second test case it is possible to replace $5$ by $1$. After that the array $a$ is $[0,\, 2,\, 4,\, 1]$, $\operatorname{DIFF} = 4$, $\operatorname{MEX} = \operatorname{MEX}(\{0, 1, 2, 4\}) = 3$, so the answer is $1$.</p><p>In the third test case one possible array $a$ is $[4,\, 13,\, 0,\, 0,\, 13,\, 1,\, 2]$, $\operatorname{DIFF} = 5$, $\operatorname{MEX} = 3$.</p><p>In the fourth test case one possible array $a$ is $[1,\, 2,\, 3,\, 0,\, 0,\, 0]$.</p>
