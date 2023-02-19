## Description

<div><p>You are given an array of $n$ non-negative integers $a_1, a_2, \ldots, a_n$. You can make the following operation: choose an integer $x \geq 2$ and replace each number of the array by the remainder when dividing that number by $x$, that is, for all $1 \leq i \leq n$ set $a_i$ to $a_i \bmod x$.</p><p>Determine if it is possible to make all the elements of the array equal by applying the operation zero or more times.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$) where $a_i$ is the $i$-th element of the array.</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a line with <span class="tex-font-style-tt">YES</span> if you can make all elements of the list equal by applying the operation. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, "YES", "Yes", "yes", "yEs" will all be recognized as a positive answer).</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 10^5$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$) where $a_i$ is the $i$-th element of the array.</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a line with <span class="tex-font-style-tt">YES</span> if you can make all elements of the list equal by applying the operation. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You may print each letter in any case (for example, "YES", "Yes", "yes", "yEs" will all be recognized as a positive answer).</p>





```input1
4
4
2 5 6 8
3
1 1 1
5
4 1 7 0 8
4
5 9 17 5
```




```output1
YES
YES
NO
YES
```



## Note

<p>In the first test case, one can apply the operation with $x = 3$ to obtain the array $[2, 2, 0, 2]$, and then apply the operation with $x = 2$ to obtain $[0, 0, 0, 0]$.</p><p>In the second test case, all numbers are already equal.</p><p>In the fourth test case, applying the operation with $x = 4$ results in the array $[1, 1, 1, 1]$.</p>
