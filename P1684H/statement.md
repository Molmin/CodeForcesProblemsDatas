## Description

<div><p>You are given a binary string $s$. You have to cut it into any number of non-intersecting substrings, so that the sum of binary integers denoted by these substrings is a power of 2. Each element of $s$ should be in exactly one substring.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>Each test case contains a binary string $s$ ($1 \le |s| \le 10^6$).</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case output the answer to the problem as follows: </p><ul> <li> If the answer does not exist, output $-1$. </li><li> If the answer exists, firstly output an integer $k$&nbsp;— the number of substrings in the answer. After that output $k$ non-intersecting substrings, for $i$-th substring output two integers $l_i, r_i$ ($1 \le l_i, r_i \le |s|$)&nbsp;— the description of $i$-th substring. </li></ul><p>If there are multiple valid solutions, you can output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). Description of the test cases follows.</p><p>Each test case contains a binary string $s$ ($1 \le |s| \le 10^6$).</p><p>It is guaranteed that the sum of $|s|$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case output the answer to the problem as follows: </p><ul> <li> If the answer does not exist, output $-1$. </li><li> If the answer exists, firstly output an integer $k$&nbsp;— the number of substrings in the answer. After that output $k$ non-intersecting substrings, for $i$-th substring output two integers $l_i, r_i$ ($1 \le l_i, r_i \le |s|$)&nbsp;— the description of $i$-th substring. </li></ul><p>If there are multiple valid solutions, you can output any of them.</p>





```input1
4
00000
01101
0111011001011
000111100111110
```




```output1
-1

3
1 3
4 4
5 5

8
1 2
3 3
4 4
5 6
7 7
8 10
11 12
13 13

5
1 5
6 7
8 11
12 14
15 15
```



## Note

<p>In the first test case it is impossible to cut the string into substrings, so that the sum is a power of 2.</p><p>In the second test case such cut is valid: </p><ul> <li> $011_2 = 3_{10}$, </li><li> $0_2 = 0_{10}$, </li><li> $1_2 = 1_{10}$. </li></ul> $3 + 0 + 1 = 4$, $4$ is a power of 2.
