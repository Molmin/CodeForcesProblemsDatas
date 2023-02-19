## Description

<div><p>You are given an integer $n$. Pair the integers $1$ to $2n$ (i.e. each integer should be in exactly one pair) so that each sum of matched pairs is consecutive and distinct. </p><p>Formally, let $(a_i, b_i)$ be the pairs that you matched. $\{a_1, b_1, a_2, b_2, \ldots, a_n, b_n\}$ should be a permutation of $\{1, 2, \ldots, 2n\}$. Let the sorted list of $\{a_1+b_1, a_2+b_2, \ldots, a_n+b_n\}$ be $s_1 &lt; s_2 &lt; \ldots &lt; s_n$. We must have $s_{i+1}-s_i = 1$ for $1 \le i \le n - 1$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>For each test case, a single integer $n$ ($1 \leq n \leq 10^5$) is given.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if it is impossible to make such a pairing, print "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">Yes</span>" followed by $n$ lines.</p><p>At each line, print two integers that are paired.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). The description of the test cases follows.</p><p>For each test case, a single integer $n$ ($1 \leq n \leq 10^5$) is given.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, if it is impossible to make such a pairing, print "<span class="tex-font-style-tt">No</span>".</p><p>Otherwise, print "<span class="tex-font-style-tt">Yes</span>" followed by $n$ lines.</p><p>At each line, print two integers that are paired.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p><p>If there are multiple solutions, print any.</p>





```input1
4
1
2
3
4
```




```output1
Yes
1 2
No
Yes
1 6
3 5
4 2
No
```



## Note

<p>For the third test case, each integer from $1$ to $6$ appears once. The sums of matched pairs are $4+2=6$, $1+6=7$, and $3+5=8$, which are consecutive and distinct.</p>
