## Description

<div><p>Consider an array $a$ of $n$ positive integers.</p><p>You may perform the following operation: </p><ul> <li> select two indices $l$ and $r$ ($1 \leq l \leq r \leq n$), then </li><li> decrease all elements $a_l, a_{l + 1}, \dots, a_r$ by $1$. </li></ul><p>Let's call $f(a)$ the minimum number of operations needed to change array $a$ into an array of $n$ zeros.</p><p>Determine if for all permutations$^\dagger$ $b$ of $a$, $f(a) \leq f(b)$ is true. </p><p>$^\dagger$ An array $b$ is a permutation of an array $a$ if $b$ consists of the elements of $a$ in arbitrary order. For example, $[4,2,3,4]$ is a permutation of $[3,2,4,4]$ while $[1,2,2]$ is not a permutation of $[1,2,3]$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$) — the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — description of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if for all permutations $b$ of $a$, $f(a) \leq f(b)$ is true, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^5$) — the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — description of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if for all permutations $b$ of $a$, $f(a) \leq f(b)$ is true, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,3,6,7
3
4
2 3 5 4
3
1 2 3
4
3 1 3 2
```




```output1
YES
YES
NO
```



## Note

<p>In the first test case, we can change all elements to $0$ in $5$ operations. It can be shown that no permutation of $[2, 3, 5, 4]$ requires less than $5$ operations to change all elements to $0$.</p><p>In the third test case, we need $5$ operations to change all elements to $0$, while $[2, 3, 3, 1]$ only needs $3$ operations.</p>
