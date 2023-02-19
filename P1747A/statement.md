## Description

<div><p>You are given an array $a$ consisting of $n$ integers. You want to distribute these $n$ integers into two groups $s_1$ and $s_2$ (groups can be empty) so that the following conditions are satisfied:</p><ul> <li> For each $i$ $(1 \leq i \leq n)$, $a_i$ goes into exactly one group.</li><li> The value $|sum(s_1)| - |sum(s_2)|$ is the maximum possible among all such ways to distribute the integers.<p>Here $sum(s_1)$ denotes the sum of the numbers in the group $s_1$, and $sum(s_2)$ denotes the sum of the numbers in the group $s_2$.</p></li></ul><p>Determine the maximum possible value of $|sum(s_1)| - |sum(s_2)|$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 2 \cdot 10^4)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1 \leq n \leq 10^5)$ &nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2 \ldots a_n$ $(-10^9 \leq a_i \leq 10^9)$ &nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the maximum possible value of $|sum(s_1)| - |sum(s_2)|$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 2 \cdot 10^4)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(1 \leq n \leq 10^5)$ &nbsp;— the length of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1,a_2 \ldots a_n$ $(-10^9 \leq a_i \leq 10^9)$ &nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the maximum possible value of $|sum(s_1)| - |sum(s_2)|$.</p>





```input1|2,3,6,7
4
2
10 -10
4
-2 -1 11 0
3
2 3 2
5
-9 2 0 0 -4
```




```output1
0
8
7
11
```



## Note

<p>In the <span class="tex-font-style-bf">first testcase</span>, we can distribute as $s_1 = \{10\}$, $s_2 = \{-10\}$. Then the value will be $|10| - |-10| = 0$.</p><p>In the <span class="tex-font-style-bf">second testcase</span>, we can distribute as $s_1 = \{0, 11, -1\}$, $s_2 = \{-2\}$. Then the value will be $|0 + 11 - 1| - |-2| = 10 - 2 = 8$.</p><p>In the <span class="tex-font-style-bf">third testcase</span>, we can distribute as $s_1 = \{2, 3, 2\}$, $s_2 = \{\}$. Then the value will be $|2 + 3 + 2| - |0| = 7$.</p><p>In the <span class="tex-font-style-bf">fourth testcase</span>, we can distribute as $s_1 = \{-9, -4, 0\}$, $s_2 = \{2, 0\}$. Then the value will be $|-9 - 4 + 0| - |2 + 0| = 13 - 2 = 11$.</p>
