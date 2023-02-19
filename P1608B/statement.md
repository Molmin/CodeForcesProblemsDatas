## Description

<div><p>You are given three integers $n, a, b$. Determine if there exists a permutation $p_1, p_2, \ldots, p_n$ of integers from $1$ to $n$, such that:</p><ul><li><p>There are exactly $a$ integers $i$ with $2 \le i \le n-1$ such that $p_{i-1} &lt; p_i &gt; p_{i+1}$ (in other words, there are exactly $a$ local maximums).</p></li><li><p>There are exactly $b$ integers $i$ with $2 \le i \le n-1$ such that $p_{i-1} &gt; p_i &lt; p_{i+1}$ (in other words, there are exactly $b$ local minimums).</p></li></ul><p>If such permutations exist, find any such permutation.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains three integers $n$, $a$ and $b$ ($2 \leq n \leq 10^5$, $0 \leq a,b \leq n$).</p><p>The sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if there is no permutation with the requested properties, output $-1$.</p><p>Otherwise, print the permutation that you are found. If there are several such permutations, you may print any of them.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains three integers $n$, $a$ and $b$ ($2 \leq n \leq 10^5$, $0 \leq a,b \leq n$).</p><p>The sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, if there is no permutation with the requested properties, output $-1$.</p><p>Otherwise, print the permutation that you are found. If there are several such permutations, you may print any of them.</p>





```input1
3
4 1 1
6 1 2
6 4 0
```




```output1
1 3 2 4
4 2 3 1 5 6
-1
```



## Note

<p>In the first test case, one example of such permutations is $[1, 3, 2, 4]$. In it $p_1 &lt; p_2 &gt; p_3$, and $2$ is the only such index, and $p_2&gt; p_3 &lt; p_4$, and $3$ the only such index.</p><p>One can show that there is no such permutation for the third test case.</p>
