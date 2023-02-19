## Description

<div><p>You are given an array $a$ of $n$ non-negative integers, numbered from $1$ to $n$.</p><p>Let's define the <span class="tex-font-style-it">cost</span> of the array $a$ as $\displaystyle \min_{i \neq j} a_i | a_j$, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>.</p><p>There are $q$ queries. For each query you are given two integers $l$ and $r$ ($l &lt; r$). For each query you should find the cost of the subarray $a_{l}, a_{l + 1}, \ldots, a_{r}$.</p></div><div class="input-specification"><p>Each test case consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 10^5$)&nbsp;— the length array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;— the elements of $a$.</p><p>The third line of each test case contains an integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains two integers $l_j$, $r_j$ ($1 \le l_j &lt; r_j \le n$)&nbsp;— the description of the $j$-th query.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases do not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print $q$ numbers, where the $j$-th number is the cost of array $a_{l_j}, a_{l_j + 1}, \ldots, a_{r_j}$.</p></div>

## Input

<p>Each test case consists of several test cases. The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 10^5$)&nbsp;— the length array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^{30}$)&nbsp;— the elements of $a$.</p><p>The third line of each test case contains an integer $q$ ($1 \le q \le 10^5$)&nbsp;— the number of queries.</p><p>Each of the next $q$ lines contains two integers $l_j$, $r_j$ ($1 \le l_j &lt; r_j \le n$)&nbsp;— the description of the $j$-th query.</p><p>It is guaranteed that the sum of $n$ and the sum of $q$ over all test cases do not exceed $10^5$.</p>

## Output

<p>For each test case print $q$ numbers, where the $j$-th number is the cost of array $a_{l_j}, a_{l_j + 1}, \ldots, a_{r_j}$.</p>





```input1
2
5
6 1 3 2 1
4
1 2
2 3
2 4
2 5
4
0 2 1 1073741823
4
1 2
2 3
1 3
3 4
```




```output1
7
3
3
1
2
3
1
1073741823
```



## Note

<p>In the first test case the array $a$ is</p><p>$110_2, 001_2, 011_2, 010_2, 001_2$.</p><p>That's why the answers for the queries are:</p><ul> <li> $[1; 2]$: $a_1 | a_2 = 110_2 | 001_2 = 111_2 = 7$; </li><li> $[2; 3]$: $a_2 | a_3 = 001_2 | 011_2 = 011_2 = 3$; </li><li> $[2; 4]$: $a_2 | a_3 = a_3 | a_4 = a_2 | a_4 = 011_2 = 3$; </li><li> $[2; 5]$: $a_2 | a_5 = 001_2 = 1$. </li></ul><p>In the second test case the array $a$ is</p><p>$00_2, 10_2, 01_2, \underbrace{11\ldots 1_2}_{30}$ ($a_4 = 2^{30} - 1$).</p><p>That's why the answers for the queries are:</p><ul> <li> $[1; 2]$: $a_1 | a_2 = 10_2 = 2$; </li><li> $[2; 3]$: $a_2 | a_3 = 11_2 = 3$; </li><li> $[1; 3]$: $a_1 | a_3 = 01_2 = 1$; </li><li> $[3; 4]$: $a_3 | a_4 = 01_2 | \underbrace{11\ldots 1_2}_{30} = 2^{30} - 1 = 1073741823$. </li></ul>
