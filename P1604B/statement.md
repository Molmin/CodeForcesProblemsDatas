## Description

<div><p>YouKn0wWho has an integer sequence $a_1, a_2, \ldots a_n$. Now he will split the sequence $a$ into one or more consecutive subarrays so that each element of $a$ belongs to exactly one subarray. Let $k$ be the number of resulting subarrays, and $h_1, h_2, \ldots, h_k$ be the lengths of the longest increasing subsequences of corresponding subarrays.</p><p>For example, if we split $[2, 5, 3, 1, 4, 3, 2, 2, 5, 1]$ into $[2, 5, 3, 1, 4]$, $[3, 2, 2, 5]$, $[1]$, then $h = [3, 2, 1]$.</p><p>YouKn0wWho wonders if it is possible to split the sequence $a$ in such a way that the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of $h_1, h_2, \ldots, h_k$ is equal to $0$. You have to tell whether it is possible.</p><p>The longest increasing subsequence (LIS) of a sequence $b_1, b_2, \ldots, b_m$ is the longest sequence of valid indices $i_1, i_2, \ldots, i_k$ such that $i_1 \lt i_2 \lt \ldots \lt i_k$ and $b_{i_1} \lt b_{i_2} \lt \ldots \lt b_{i_k}$. For example, the LIS of $[2, 5, 3, 3, 5]$ is $[2, 3, 5]$, which has length $3$.</p><p>An array $c$ is a subarray of an array $b$ if $c$ can be obtained from $b$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to split into subarrays in the desired way, print "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can print each letter in any register (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10\,000$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to split into subarrays in the desired way, print "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. You can print each letter in any register (upper or lower).</p>





```input1
4
7
1 3 4 2 2 1 5
3
1 3 4
5
1 3 2 4 2
4
4 3 2 1
```




```output1
YES
NO
YES
YES
```



## Note

<p>In the first test case, YouKn0wWho can split the sequence in the following way: $[1, 3, 4]$, $[2, 2]$, $[1, 5]$. This way, the LIS lengths are $h = [3, 1, 2]$, and the bitwise XOR of the LIS lengths is $3 \oplus 1 \oplus 2 = 0$.</p><p>In the second test case, it can be shown that it is impossible to split the sequence into subarrays that will satisfy the condition.</p>
