## Description

<div><p>Given an array $a$ consisting of $n$ elements, find the maximum possible sum the array can have after performing the following operation <span class="tex-font-style-bf">any number of times</span>: </p><ul> <li> Choose $2$ <span class="tex-font-style-bf">adjacent</span> elements and flip both of their signs. In other words choose an index $i$ such that $1 \leq i \leq n - 1$ and assign $a_i = -a_i$ and $a_{i+1} = -a_{i+1}$. </li></ul></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated integers $a_1,a_2,\dots,a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum possible sum the array can have after performing the described operation any number of times.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated integers $a_1,a_2,\dots,a_n$ ($-10^9 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output the maximum possible sum the array can have after performing the described operation any number of times.</p>





```input1|2,3,6,7,10,11
5
3
-1 -1 -1
5
1 5 -5 0 2
3
1 2 3
6
-1 10 9 8 7 6
2
-1 -1
```




```output1
1
13
6
39
2
```



## Note

<p>For the first test case, by performing the operation on the first two elements, we can change the array from $[-1, -1, -1]$ to $[1, 1, -1]$, and it can be proven this array obtains the maximum possible sum which is $1 + 1 + (-1) = 1$.</p><p>For the second test case, by performing the operation on $-5$ and $0$, we change the array from $[1, 5, -5, 0, 2]$ to $[1, 5, -(-5), -0, 2] = [1, 5, 5, 0, 2]$, which has the maximum sum since all elements are non-negative. So, the answer is $1 + 5 + 5 + 0 + 2 = 13$.</p><p>For the third test case, the array already contains only positive numbers, so performing operations is unnecessary. The answer is just the sum of the whole array, which is $1 + 2 + 3 = 6$.</p>
