## Description

<div><p>You are given an array $a$ of size $n$. Each element in this array is an integer between $1$ and $10^9$.</p><p>You can perform several operations to this array. During an operation, you can replace an element in the array with any integer between $1$ and $10^9$. </p><p>Output the minimum number of operations needed such that the resulting array doesn't contain any local maximums, and the resulting array after the operations.</p><p>An element $a_i$ is a local maximum if it is strictly larger than both of its neighbors (that is, $a_i &gt; a_{i - 1}$ and $a_i &gt; a_{i + 1}$). Since $a_1$ and $a_n$ have only one neighbor each, they will never be a local maximum.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line will contain a single integer $t$ $(1 \leq t \leq 10000)$ — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ $(2 \leq n \leq 2 \cdot 10^5)$ — the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots ,a_n$ $(1 \leq a_i \leq 10^9)$, the elements of array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, first output a line containing a single integer $m$ — minimum number of operations required. Then ouput a line consist of $n$ integers — the resulting array after the operations. Note that this array should differ in exactly $m$ elements from the initial array.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line will contain a single integer $t$ $(1 \leq t \leq 10000)$ — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ $(2 \leq n \leq 2 \cdot 10^5)$ — the size of the array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots ,a_n$ $(1 \leq a_i \leq 10^9)$, the elements of array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, first output a line containing a single integer $m$ — minimum number of operations required. Then ouput a line consist of $n$ integers — the resulting array after the operations. Note that this array should differ in exactly $m$ elements from the initial array.</p><p>If there are multiple answers, print any.</p>





```input1
5
3
2 1 2
4
1 2 3 1
5
1 2 1 2 1
9
1 2 1 3 2 3 1 2 1
9
2 1 3 1 3 1 3 1 3
```




```output1
0
2 1 2
1
1 3 3 1
1
1 2 2 2 1
2
1 2 3 3 2 3 3 2 1
2
2 1 3 3 3 1 1 1 3
```



## Note

<p>In the first example, the array contains no local maximum, so we don't need to perform operations.</p><p>In the second example, we can change $a_2$ to $3$, then the array don't have local maximums.</p>
