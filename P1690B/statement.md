## Description

<div><p>Kristina has two arrays $a$ and $b$, each containing $n$ non-negative integers. She can perform the following operation on array $a$ any number of times: </p><ul> <li> apply a decrement to each non-zero element of the array, that is, replace the value of each element $a_i$ such that $a_i &gt; 0$ with the value $a_i - 1$ ($1 \le i \le n$). If $a_i$ was $0$, its value does not change. </li></ul><p>Determine whether Kristina can get an array $b$ from an array $a$ in some number of operations (probably zero). In other words, can she make $a_i = b_i$ after some number of operations for each $1 \le i \le n$?</p><p>For example, let $n = 4$, $a = [3, 5, 4, 1]$ and $b = [1, 3, 2, 0]$. In this case, she can apply the operation twice: </p><ul> <li> after the first application of the operation she gets $a = [2, 4, 3, 0]$; </li><li> after the second use of the operation she gets $a = [1, 3, 2, 0]$. </li></ul><p>Thus, in two operations, she can get an array $b$ from an array $a$.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^4$).</p><p>The second line of each test case contains exactly $n$ non-negative integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p><p>The third line of each test case contains exactly $n$ non-negative integers $b_1, b_2, \dots, b_n$ ($0 \le b_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ values over all test cases in the test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span>, if by doing some number of operations it is possible to get an array $b$ from an array $a$; </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^4$).</p><p>The second line of each test case contains exactly $n$ non-negative integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p><p>The third line of each test case contains exactly $n$ non-negative integers $b_1, b_2, \dots, b_n$ ($0 \le b_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ values over all test cases in the test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span>, if by doing some number of operations it is possible to get an array $b$ from an array $a$; </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p>





```input1
6
4
3 5 4 1
1 3 2 0
3
1 2 1
0 1 0
4
5 3 7 2
1 1 1 1
5
1 2 3 4 5
1 2 3 4 6
1
8
0
1
4
6
```




```output1
YES
YES
NO
NO
YES
NO
```



## Note

<p>The first test case is analyzed in the statement.</p><p>In the second test case, it is enough to apply the operation to array $a$ once.</p><p>In the third test case, it is impossible to get array $b$ from array $a$.</p>
