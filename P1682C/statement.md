## Description

<div><p>You are given an array $a$ of $n$ positive integers. </p><p>Let $\text{LIS}(a)$ denote the length of <a href="https://en.wikipedia.org/wiki/Longest_increasing_subsequence">longest strictly increasing subsequence</a> of $a$. For example,</p><ul> <li> $\text{LIS}([2, \underline{1}, 1, \underline{3}])$ = $2$. </li><li> $\text{LIS}([\underline{3}, \underline{5}, \underline{10}, \underline{20}])$ = $4$. </li><li> $\text{LIS}([3, \underline{1}, \underline{2}, \underline{4}])$ = $3$. </li></ul> <p>We define array $a'$ as the array obtained after reversing the array $a$ i.e. $a' = [a_n, a_{n-1}, \ldots , a_1]$.</p><p>The beauty of array $a$ is defined as $min(\text{LIS}(a),\text{LIS}(a'))$.</p><p>Your task is to determine the maximum possible beauty of the array $a$ if you can rearrange the array $a$ arbitrarily.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 10^4)$ &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1 \leq n \leq 2\cdot 10^5)$ &nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2, \ldots ,a_n$ $(1 \leq a_i \leq 10^9)$ &nbsp;— the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the maximum possible beauty of $a$ after rearranging its elements arbitrarily.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 10^4)$ &nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1 \leq n \leq 2\cdot 10^5)$ &nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2, \ldots ,a_n$ $(1 \leq a_i \leq 10^9)$ &nbsp;— the elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the maximum possible beauty of $a$ after rearranging its elements arbitrarily.</p>





```input1
3
3
6 6 6
6
2 5 4 5 2 4
4
1 3 2 2
```




```output1
1
3
2
```



## Note

<p>In the first test case, $a$ = $[6, 6, 6]$ and $a'$ = $[6, 6, 6]$. $\text{LIS}(a) = \text{LIS}(a')$ = $1$. Hence the beauty is $min(1, 1) = 1$.</p><p>In the second test case, $a$ can be rearranged to $[2, 5, 4, 5, 4, 2]$. Then $a'$ = $[2, 4, 5, 4, 5, 2]$. $\text{LIS}(a) = \text{LIS}(a') = 3$. Hence the beauty is $3$ and it can be shown that this is the maximum possible beauty.</p><p>In the third test case, $a$ can be rearranged to $[1, 2, 3, 2]$. Then $a'$ = $[2, 3, 2, 1]$. $\text{LIS}(a) = 3$, $\text{LIS}(a') = 2$. Hence the beauty is $min(3, 2) = 2$ and it can be shown that $2$ is the maximum possible beauty.</p>
