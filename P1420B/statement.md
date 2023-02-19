## Description

<div><div class="epigraph"><div class="epigraph-text"> <span class="tex-font-size-small"> "You must lift the dam. With a lever. I will give it to you.<p>You must block the canal. With a rock. I will not give the rock to you." </p></span></div></div><p>Danik urgently needs rock and lever! Obviously, the easiest way to get these things is to ask Hermit Lizard for them.</p><p>Hermit Lizard agreed to give Danik the lever. But to get a stone, Danik needs to solve the following task.</p><p>You are given a positive integer $n$, and an array $a$ of positive integers. The task is to calculate the number of such pairs $(i,j)$ that $i&lt;j$ and $a_i$ $\&amp;$ $a_j \ge a_i \oplus a_j$, where $\&amp;$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND operation</a>, and $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Danik has solved this task. But can you solve it?</p></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10$) denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $n$ ($1 \le n \le 10^5$)&nbsp;— length of the array.</p><p>The second line contains $n$ positive integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For every test case print one non-negative integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10$) denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $n$ ($1 \le n \le 10^5$)&nbsp;— length of the array.</p><p>The second line contains $n$ positive integers $a_i$ ($1 \le a_i \le 10^9$)&nbsp;— elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For every test case print one non-negative integer&nbsp;— the answer to the problem.</p>





```input1
5
5
1 4 3 7 10
3
1 1 1
4
6 2 5 3
2
2 4
1
1
```




```output1
1
3
2
0
0
```



## Note

<p>In the first test case there is only one pair: $(4,7)$: for it $4$ $\&amp;$ $7 = 4$, and $4 \oplus 7 = 3$.</p><p>In the second test case all pairs are good.</p><p>In the third test case there are two pairs: $(6,5)$ and $(2,3)$.</p><p>In the fourth test case there are no good pairs.</p>
