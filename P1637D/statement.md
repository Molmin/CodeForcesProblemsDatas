## Description

<div><p>You are given two arrays $a$ and $b$, both of length $n$.</p><p>You can perform the following operation any number of times (possibly zero): select an index $i$ ($1 \leq i \leq n$) and swap $a_i$ and $b_i$.</p><p>Let's define the <span class="tex-font-style-it">cost</span> of the array $a$ as $\sum_{i=1}^{n} \sum_{j=i + 1}^{n} (a_i + a_j)^2$. Similarly, the <span class="tex-font-style-it">cost</span> of the array $b$ is $\sum_{i=1}^{n} \sum_{j=i + 1}^{n} (b_i + b_j)^2$.</p><p>Your task is to minimize the total <span class="tex-font-style-it">cost</span> of two arrays.</p></div><div class="input-specification"><p>Each test case consists of several test cases. The first line contains a single integer $t$ ($1 \leq t \leq 40$)&nbsp;— the number of test cases. The following is a description of the input data sets.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of both arrays.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$)&nbsp;— elements of the first array.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 100$)&nbsp;— elements of the second array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p></div><div class="output-specification"><p>For each test case, print the minimum possible total cost.</p></div>

## Input

<p>Each test case consists of several test cases. The first line contains a single integer $t$ ($1 \leq t \leq 40$)&nbsp;— the number of test cases. The following is a description of the input data sets.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of both arrays.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 100$)&nbsp;— elements of the first array.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 100$)&nbsp;— elements of the second array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $100$.</p>

## Output

<p>For each test case, print the minimum possible total cost.</p>





```input1
3
1
3
6
4
3 6 6 6
2 7 4 1
4
6 7 2 4
2 5 3 5
```




```output1
0
987
914
```



## Note

<p>In the second test case, in one of the optimal answers after all operations $a = [2, 6, 4, 6]$, $b = [3, 7, 6, 1]$.</p><p>The cost of the array $a$ equals to $(2 + 6)^2 + (2 + 4)^2 + (2 + 6)^2 + (6 + 4)^2 + (6 + 6)^2 + (4 + 6)^2 = 508$.</p><p>The cost of the array $b$ equals to $(3 + 7)^2 + (3 + 6)^2 + (3 + 1)^2 + (7 + 6)^2 + (7 + 1)^2 + (6 + 1)^2 = 479$.</p><p>The total cost of two arrays equals to $508 + 479 = 987$.</p>
