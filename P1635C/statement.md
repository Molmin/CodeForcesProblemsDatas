## Description

<div><p>You are given an array $a$ of $n$ elements. </p><p>Your can perform the following operation no more than $n$ times: Select three indices $x,y,z$ $(1 \leq x &lt; y &lt; z \leq n)$ and replace $a_x$ with $a_y - a_z$. After the operation, $|a_x|$ need to be less than $10^{18}$.</p><p>Your goal is to make the resulting array <span class="tex-font-style-bf">non-decreasing</span>. If there are multiple solutions, you can output any. If it is impossible to achieve, you should report it as well.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line will contain a single integer $t$ $(1 \leq t \leq 10000)$ — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ $(3 \leq n \leq 2 \cdot 10^5)$ — the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots ,a_n$ $(-10^9 \leq a_i \leq 10^9)$, the elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $-1$ in a single line if there is no solution. Otherwise in the first line you should print a single integer $m$ $(0 \leq m \leq n)$ — number of operations you performed.</p><p>Then the $i$-th of the following $m$ lines should contain three integers $x,y,z$ $(1 \leq x &lt; y &lt; z \leq n)$— description of the $i$-th operation.</p><p>If there are multiple solutions, you can output any. Note that you don't have to minimize the number of operations in this task.</p></div>

## Input

<p>Each test contains multiple test cases. The first line will contain a single integer $t$ $(1 \leq t \leq 10000)$ — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ $(3 \leq n \leq 2 \cdot 10^5)$ — the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots ,a_n$ $(-10^9 \leq a_i \leq 10^9)$, the elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $-1$ in a single line if there is no solution. Otherwise in the first line you should print a single integer $m$ $(0 \leq m \leq n)$ — number of operations you performed.</p><p>Then the $i$-th of the following $m$ lines should contain three integers $x,y,z$ $(1 \leq x &lt; y &lt; z \leq n)$— description of the $i$-th operation.</p><p>If there are multiple solutions, you can output any. Note that you don't have to minimize the number of operations in this task.</p>





```input1
3
5
5 -4 2 -1 2
3
4 3 2
3
-3 -2 -1
```




```output1
2
1 2 3
3 4 5
-1
0
```



## Note

<p>In the first example, the array becomes </p><p>$[-6,-4,2,-1,2]$ after the first operation,</p><p>$[-6,-4,-3,-1,2]$ after the second operation.</p><p>In the second example, it is impossible to make the array sorted after any sequence of operations.</p><p>In the third example, the array is already sorted, so we don't need to perform any operations.</p>
