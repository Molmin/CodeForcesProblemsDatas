## Description

<div><p>You are given a sequence $a$ of length $n$ consisting of $0$s and $1$s.</p><p>You can perform the following operation on this sequence: </p><ul> <li> Pick an index $i$ from $1$ to $n-2$ (inclusive). </li><li> Change all of $a_{i}$, $a_{i+1}$, $a_{i+2}$ to $a_{i} \oplus a_{i+1} \oplus a_{i+2}$ simultaneously, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a> </li></ul> Find a sequence of <span class="tex-font-style-bf">at most</span> $n$ operations that changes all elements of $a$ to $0$s or report that it's impossible.<p>We can prove that if there exists a sequence of operations of any length that changes all elements of $a$ to $0$s, then there is also such a sequence of length not greater than $n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$).</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2\cdot10^5$) — the length of $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i = 0$ or $a_i = 1$) — elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, do the following: </p><ul> <li> if there is no way of making all the elements of $a$ equal to $0$ after performing the above operation some number of times, print "<span class="tex-font-style-tt">NO</span>". </li><li> otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>", in the second line print $k$ ($0 \le k \le n$) — the number of operations that you want to perform on $a$, and in the third line print a sequence $b_1, b_2, \dots, b_k$ ($1 \le b_i \le n - 2$) — the indices on which the operation should be applied. </li></ul><p>If there are multiple solutions, you may print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$).</p><p>The first line of each test case contains a single integer $n$ ($3 \le n \le 2\cdot10^5$) — the length of $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i = 0$ or $a_i = 1$) — elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, do the following: </p><ul> <li> if there is no way of making all the elements of $a$ equal to $0$ after performing the above operation some number of times, print "<span class="tex-font-style-tt">NO</span>". </li><li> otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>", in the second line print $k$ ($0 \le k \le n$) — the number of operations that you want to perform on $a$, and in the third line print a sequence $b_1, b_2, \dots, b_k$ ($1 \le b_i \le n - 2$) — the indices on which the operation should be applied. </li></ul><p>If there are multiple solutions, you may print any.</p>





```input1
3
3
0 0 0
5
1 1 1 1 0
4
1 0 0 1
```




```output1
YES
0
YES
2
3 1
NO
```



## Note

<p>In the first example, the sequence contains only $0$s so we don't need to change anything.</p><p>In the second example, we can transform $[1, 1, 1, 1, 0]$ to $[1, 1, 0, 0, 0]$ and then to $[0, 0, 0, 0, 0]$ by performing the operation on the third element of $a$ and then on the first element of $a$.</p><p>In the third example, no matter whether we first perform the operation on the first or on the second element of $a$ we will get $[1, 1, 1, 1]$, which cannot be transformed to $[0, 0, 0, 0]$.</p>
