## Description

<div><p>There is an array $a$ of length $n$. You may perform the following operation any number of times:</p><ul> <li> Choose two indices $l$ and $r$ where $1 \le l &lt; r \le n$ and $a_l = a_r$. Then, set $a[l \ldots r] = [a_{l+1}, a_{l+2}, \ldots, a_r, a_l]$. </li></ul><p>You are also given another array $b$ of length $n$ which is a permutation of $a$. Determine whether it is possible to transform array $a$ into an array $b$ using the above operation some number of times.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10 ^ 5$) &nbsp;— the length of array $a$ and $b$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) &nbsp;— elements of the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$) &nbsp;— elements of the array $b$.</p><p>It is guaranteed that $b$ is a permutation of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to transform array $a$ to $b$, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10 ^ 5$) &nbsp;— the length of array $a$ and $b$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$) &nbsp;— elements of the array $a$.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le n$) &nbsp;— elements of the array $b$.</p><p>It is guaranteed that $b$ is a permutation of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10 ^ 5$</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to transform array $a$ to $b$, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1
5
5
1 2 3 3 2
1 3 3 2 2
5
1 2 4 2 1
4 2 2 1 1
5
2 4 5 5 2
2 2 4 5 5
3
1 2 3
1 2 3
3
1 1 2
2 1 1
```




```output1
YES
YES
NO
YES
NO
```



## Note

<p>In the first test case, we can choose $l=2$ and $r=5$ to form $[1, 3, 3, 2, 2]$.</p><p>In the second test case, we can choose $l=2$ and $r=4$ to form $[1, 4, 2, 2, 1]$. Then, we can choose $l=1$ and $r=5$ to form $[4, 2, 2, 1, 1]$.</p><p>In the third test case, it can be proven that it is not possible to transform array $a$ to $b$ using the operation.</p>
