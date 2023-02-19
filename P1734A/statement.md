## Description

<div><p>You are given $n$ sticks with positive integral length $a_1, a_2, \ldots, a_n$.</p><p>You can perform the following operation any number of times (possibly zero): </p><ul> <li> choose one stick, then either increase or decrease its length by $1$. After each operation, all sticks should have positive lengths. </li></ul><p>What is the minimum number of operations that you have to perform such that it is possible to select three of the $n$ sticks and use them without breaking to form an <span class="tex-font-style-it">equilateral triangle</span>?</p><p>An <span class="tex-font-style-it">equilateral triangle</span> is a triangle where all of its three sides have the same length.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 300$)&nbsp;— the number of sticks.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the lengths of the sticks.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $300$. </p></div><div class="output-specification"><p>For each test case, print one integer on a single line&nbsp;— the minimum number of operations to be made.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 300$)&nbsp;— the number of sticks.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the lengths of the sticks.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $300$. </p>

## Output

<p>For each test case, print one integer on a single line&nbsp;— the minimum number of operations to be made.</p>





```input1|2,3,6,7
4
3
1 2 3
4
7 3 7 3
5
3 4 2 1 1
8
3 1 4 1 5 9 2 6
```




```output1
2
4
1
1
```



## Note

<p>In the first test case, you can increase the length of the first stick by $1$, then decrease the length of the third stick by $1$. In total, you perform $2$ operations, such that the three sticks form an equilateral triangle of side length $2$.</p><p>In the fourth test case, you can decrease the length of the seventh stick by $1$. An equilateral triangle of side length $1$ can be selected and formed by the second, fourth, and seventh sticks.</p>
