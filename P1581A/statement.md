## Description

<div><p>CQXYM is counting permutations length of $2n$.</p><p>A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>A permutation $p$(length of $2n$) will be counted only if the number of $i$ satisfying $p_i&lt;p_{i+1}$ is no less than $n$. For example:</p><ul> <li> Permutation $[1, 2, 3, 4]$ will count, because the number of such $i$ that $p_i&lt;p_{i+1}$ equals $3$ ($i = 1$, $i = 2$, $i = 3$).</li><li> Permutation $[3, 2, 1, 4]$ won't count, because the number of such $i$ that $p_i&lt;p_{i+1}$ equals $1$ ($i = 3$). </li></ul><p>CQXYM wants you to help him to count the number of such permutations modulo $1000000007$ ($10^9+7$).</p><p>In addition, <a href="https://en.wikipedia.org/wiki/Modulo_operation">modulo operation</a> is to get the remainder. For example:</p><ul> <li> $7 \mod 3=1$, because $7 = 3 \cdot 2 + 1$, </li><li> $15 \mod 4=3$, because $15 = 4 \cdot 3 + 3$. </li></ul></div><div class="input-specification"><p>The input consists of multiple test cases. </p><p>The first line contains an integer $t (t \geq 1)$ — the number of test cases. The description of the test cases follows.</p><p>Only one line of each test case contains an integer $n(1 \leq n \leq 10^5)$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$</p></div><div class="output-specification"><p>For each test case, print the answer in a single line.</p></div>

## Input

<p>The input consists of multiple test cases. </p><p>The first line contains an integer $t (t \geq 1)$ — the number of test cases. The description of the test cases follows.</p><p>Only one line of each test case contains an integer $n(1 \leq n \leq 10^5)$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$</p>

## Output

<p>For each test case, print the answer in a single line.</p>





```input1
4
1
2
9
91234
```




```output1
1
12
830455698
890287984
```



## Note

<p>$n=1$, there is only one permutation that satisfies the condition: $[1,2].$</p><p>In permutation $[1,2]$, $p_1&lt;p_2$, and there is one $i=1$ satisfy the condition. Since $1 \geq n$, this permutation should be counted. In permutation $[2,1]$, $p_1&gt;p_2$. Because $0&lt;n$, this permutation should not be counted.</p><p>$n=2$, there are $12$ permutations: $[1,2,3,4],[1,2,4,3],[1,3,2,4],[1,3,4,2],[1,4,2,3],[2,1,3,4],[2,3,1,4],[2,3,4,1],[2,4,1,3],[3,1,2,4],[3,4,1,2],[4,1,2,3].$</p>
