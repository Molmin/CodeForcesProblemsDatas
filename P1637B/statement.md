## Description

<div><p>Let there be an array $b_1, b_2, \ldots, b_k$. Let there be a partition of this array into segments $[l_1; r_1], [l_2; r_2], \ldots, [l_c; r_c]$, where $l_1 = 1$, $r_c = k$, and for any $2 \leq i \leq c$ holds that $r_{i-1} + 1 = l_i$. In other words, each element of the array belongs to exactly one segment.</p><p>Let's define the <span class="tex-font-style-it">cost</span> of a partition as $$c + \sum_{i = 1}^{c} \operatorname{mex}(\{b_{l_i}, b_{l_i + 1}, \ldots, b_{r_i}\}),$$ where $\operatorname{mex}$ of a set of numbers $S$ is the smallest non-negative integer that does not occur in the set $S$. In other words, the <span class="tex-font-style-it">cost</span> of a partition is the number of segments plus the sum of MEX over all segments. Let's define the <span class="tex-font-style-it">value</span> of an array $b_1, b_2, \ldots, b_k$ as the <span class="tex-font-style-bf">maximum</span> possible <span class="tex-font-style-it">cost</span> over all partitions of this array.</p><p>You are given an array $a$ of size $n$. Find the sum of <span class="tex-font-style-it">values</span> of all its subsegments.</p><p>An array $x$ is a subsegment of an array $y$ if $x$ can be obtained from $y$ by deletion of several (possibly, zero or all) elements from the beginning and several (possibly, zero or all) elements from the end.</p></div><div class="input-specification"><p>The input contains several test cases. The first line contains one integer $t$ ($1 \leq t \leq 30$)&nbsp;— the number of test cases.</p><p>The first line for each test case contains one integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of the array.</p><p>The second line contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;— the array elements.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $100$.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>The input contains several test cases. The first line contains one integer $t$ ($1 \leq t \leq 30$)&nbsp;— the number of test cases.</p><p>The first line for each test case contains one integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of the array.</p><p>The second line contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 10^9$)&nbsp;— the array elements.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $100$.</p>

## Output

<p>For each test case print a single integer&nbsp;— the answer to the problem.</p>





```input1
4
2
1 2
3
2 0 1
4
2 0 5 1
5
0 1 1 0 1
```




```output1
4
14
26
48
```



## Note

<p>In the second test case: </p><ul> <li> The best partition for the subsegment $[2, 0, 1]$: $[2], [0, 1]$. The cost of this partition equals to $2 + \operatorname{mex}(\{2\}) + \operatorname{mex}(\{0, 1\}) = 2 + 0 + 2 = 4$. </li><li> The best partition for the subsegment $[2, 0]$: $[2], [0]$. The cost of this partition equals to $2 + \operatorname{mex}(\{2\}) + \operatorname{mex}(\{0\}) = 2 + 0 + 1 = 3$ </li><li> The best partition for the subsegment $[2]$: $[2]$. The cost of this partition equals to $1 + \operatorname{mex}(\{2\}) = 1 + 0 = 1$. </li><li> The best partition for the subsegment $[0, 1]$: $[0, 1]$. The cost of this partition equals to $1 + \operatorname{mex}(\{0, 1\}) = 1 + 2 = 3$. </li><li> The best partition for the subsegment $[0]$: $[0]$. The cost of this partition equals to $1 + \operatorname{mex}(\{0\}) = 1 + 1 = 2$. </li><li> The best partition for the subsegment $[1]$: $[1]$. The cost of this partition equals to $1 + \operatorname{mex}(\{1\}) = 1 + 0 = 1$. </li></ul><p>The sum of values over all subsegments equals to $4 + 3 + 1 + 3 + 2 + 1 = 14$.</p>
