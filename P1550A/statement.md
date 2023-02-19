## Description

<div><p>Let's call an array $a$ consisting of $n$ positive (greater than $0$) integers <span class="tex-font-style-it">beautiful</span> if the following condition is held for every $i$ from $1$ to $n$: either $a_i = 1$, or at least one of the numbers $a_i - 1$ and $a_i - 2$ exists in the array as well.</p><p>For example: </p><ul> <li> the array $[5, 3, 1]$ is beautiful: for $a_1$, the number $a_1 - 2 = 3$ exists in the array; for $a_2$, the number $a_2 - 2 = 1$ exists in the array; for $a_3$, the condition $a_3 = 1$ holds; </li><li> the array $[1, 2, 2, 2, 2]$ is beautiful: for $a_1$, the condition $a_1 = 1$ holds; for every other number $a_i$, the number $a_i - 1 = 1$ exists in the array; </li><li> the array $[1, 4]$ is not beautiful: for $a_2$, neither $a_2 - 2 = 2$ nor $a_2 - 1 = 3$ exists in the array, and $a_2 \ne 1$; </li><li> the array $[2]$ is not beautiful: for $a_1$, neither $a_1 - 1 = 1$ nor $a_1 - 2 = 0$ exists in the array, and $a_1 \ne 1$; </li><li> the array $[2, 1, 3]$ is beautiful: for $a_1$, the number $a_1 - 1 = 1$ exists in the array; for $a_2$, the condition $a_2 = 1$ holds; for $a_3$, the number $a_3 - 2 = 1$ exists in the array. </li></ul><p>You are given a positive integer $s$. Find the minimum possible size of a beautiful array with the sum of elements equal to $s$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5000$) — the number of test cases.</p><p>Then $t$ lines follow, the $i$-th line contains one integer $s$ ($1 \le s \le 5000$) for the $i$-th test case.</p></div><div class="output-specification"><p>Print $t$ integers, the $i$-th integer should be the answer for the $i$-th testcase: the minimum possible size of a beautiful array with the sum of elements equal to $s$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5000$) — the number of test cases.</p><p>Then $t$ lines follow, the $i$-th line contains one integer $s$ ($1 \le s \le 5000$) for the $i$-th test case.</p>

## Output

<p>Print $t$ integers, the $i$-th integer should be the answer for the $i$-th testcase: the minimum possible size of a beautiful array with the sum of elements equal to $s$.</p>





```input1
4
1
8
7
42
```




```output1
1
3
3
7
```



## Note

<p>Consider the example test:</p><ol> <li> in the first test case, the array $[1]$ meets all conditions; </li><li> in the second test case, the array $[3, 4, 1]$ meets all conditions; </li><li> in the third test case, the array $[1, 2, 4]$ meets all conditions; </li><li> in the fourth test case, the array $[1, 4, 6, 8, 10, 2, 11]$ meets all conditions. </li></ol>
