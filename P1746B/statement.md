## Description

<div><p>You have an array $a$ of size $n$ consisting only of zeroes and ones. You can do the following operation:</p><ul> <li> choose two indices $1 \le i , j \le n$, $i \ne j$, </li><li> add $a_{i}$ to $a_{j}$, </li><li> remove $a_{i}$ from $a$. </li></ul><p>Note that elements of $a$ can become bigger than $1$ after performing some operations. Also note that $n$ becomes $1$ less after the operation.</p><p>What is the minimum number of operations needed to make $a$ non-decreasing, i.&nbsp;e. that each element is not less than the previous element?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 10^5$), the size of array $a$.</p><p>Next line contains $n$ integers $a_{1}, a_{2}, \ldots a_{n}$ ($a_i$ is $0$ or $1$), elements of array $a$.</p><p>It's guaranteed that sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer, minimum number of operations needed to make $a$ non-decreasing.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 10^5$), the size of array $a$.</p><p>Next line contains $n$ integers $a_{1}, a_{2}, \ldots a_{n}$ ($a_i$ is $0$ or $1$), elements of array $a$.</p><p>It's guaranteed that sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print a single integer, minimum number of operations needed to make $a$ non-decreasing.</p>





```input1|2,3,6,7
4
8
0 0 1 1 1 1 1 1
5
1 0 0 1 1
2
1 0
11
1 1 0 0 1 0 0 1 1 1 0
```




```output1
0
1
1
3
```



## Note

<p>In the first test case, $a$ is already non-decreasing, so you don't need to do any operations and the answer is $0$.</p><p>In the second test case, you can perform an operation for $i = 1$ and $j = 5$, so $a$ will be equal to $[0, 0, 1, 2]$ and it becomes non-decreasing.</p><p>In the third test case, you can perform an operation for $i = 2$ and $j = 1$, so $a$ will be equal to $[1]$ and it becomes non-decreasing.</p>
