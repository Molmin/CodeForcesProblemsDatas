## Description

<div><p>You are given an array of exactly $n$ numbers $[1,2,3,\ldots,n]$ along with integers $k$ and $x$.</p><p>Partition the array in exactly $k$ non-empty disjoint subsequences such that the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all numbers in each subsequence is $x$, and each number is in exactly one subsequence. Notice that there are no constraints on the length of each subsequence.</p><p>A sequence $a$ is a subsequence of a sequence $b$ if $a$ can be obtained from $b$ by the deletion of several (possibly, zero or all) elements.</p><p>For example, for $n = 15$, $k = 6$, $x = 7$, the following scheme is valid: </p><ul> <li> $[6,10,11]$, $6 \oplus 10 \oplus 11 = 7$, </li><li> $[5,12,14]$, $5 \oplus 12 \oplus 14 = 7$, </li><li> $[3,9,13]$, $3 \oplus 9 \oplus 13 = 7$, </li><li> $[1,2,4]$, $1 \oplus 2 \oplus 4 = 7$, </li><li> $[8,15]$, $8 \oplus 15 = 7$, </li><li> $[7]$, $7 = 7$, </li></ul> where $\oplus$ represents the bitwise XOR operation.<p>The following scheme is invalid, since $8$, $15$ do not appear: </p><ul> <li> $[6,10,11]$, $6 \oplus 10 \oplus 11 = 7$, </li><li> $[5,12,14]$, $5 \oplus 12 \oplus 14 = 7$, </li><li> $[3,9,13]$, $3 \oplus 9 \oplus 13 = 7$, </li><li> $[1,2,4]$, $1 \oplus 2 \oplus 4 = 7$, </li><li> $[7]$, $7 = 7$. </li></ul><p>The following scheme is invalid, since $3$ appears twice, and $1$, $2$ do not appear: </p><ul> <li> $[6,10,11]$, $6 \oplus 10 \oplus 11 = 7$, </li><li> $[5,12,14]$, $5 \oplus 12 \oplus 14 = 7$, </li><li> $[3,9,13]$, $3 \oplus 9 \oplus 13 = 7$, </li><li> $[3,4]$, $3 \oplus 4 = 7$, </li><li> $[8,15]$, $8 \oplus 15 = 7$, </li><li> $[7]$, $7 = 7$. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases. </p><p>The first and the only line of each test case contains three integers $n$, $k$, $x$ ($1 \le k \le n \le 2 \cdot 10^5$; $1\le x \le 10^9$) — the length of the array, the number of subsequences and the required XOR.</p><p>It's guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if it is possible to partition the sequence, print "<span class="tex-font-style-tt">YES</span>" in the first line. In the $i$-th of the following $k$ lines first print the length $s_i$ of the $i$-th subsequence, then print $s_i$ integers, representing the elements in the $i$-th subsequence. If there are multiple answers, print any. Note that you can print a subsequence in any order.</p><p>If it is not possible to partition the sequence, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases. </p><p>The first and the only line of each test case contains three integers $n$, $k$, $x$ ($1 \le k \le n \le 2 \cdot 10^5$; $1\le x \le 10^9$) — the length of the array, the number of subsequences and the required XOR.</p><p>It's guaranteed that the sum of $n$ does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, if it is possible to partition the sequence, print "<span class="tex-font-style-tt">YES</span>" in the first line. In the $i$-th of the following $k$ lines first print the length $s_i$ of the $i$-th subsequence, then print $s_i$ integers, representing the elements in the $i$-th subsequence. If there are multiple answers, print any. Note that you can print a subsequence in any order.</p><p>If it is not possible to partition the sequence, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|2,4,6,8
7
15 6 7
11 4 5
5 3 2
4 1 4
6 1 7
11 5 5
11 6 5
```




```output1
YES
3 6 10 11
3 5 12 14
3 3 9 13
3 1 2 4
2 8 15
1 7
YES
2 1 4
2 2 7
2 3 6
5 5 8 9 10 11
NO
YES
4 1 2 3 4
YES
6 1 2 3 4 5 6
NO
NO
```



## Note

<p>In the first test case, we construct the following $6$ subsequences: </p><ul> <li> $[6,10,11]$, $6 \oplus 10 \oplus 11 = 7$, </li><li> $[5,12,14]$, $5 \oplus 12 \oplus 14 = 7$, </li><li> $[3,9,13]$, $3 \oplus 9 \oplus 13 = 7$, </li><li> $[1,2,4]$, $1 \oplus 2 \oplus 4 = 7$, </li><li> $[8,15]$, $8 \oplus 15 = 7$, </li><li> $[7]$, $7 = 7$. </li></ul><p>In the second test case, we construct the following $4$ subsequences: </p><ul> <li> $[1,4]$, $1 \oplus 4 = 5$, </li><li> $[2,7]$, $2 \oplus 7 = 5$, </li><li> $[3,6]$, $3 \oplus 6 = 5$, </li><li> $[5,8,9,10,11]$, $5 \oplus 8 \oplus 9 \oplus 10 \oplus 11 = 5$. </li></ul><p>The following solution is considered correct in this test case as well: </p><ul> <li> $[1,4]$, $1 \oplus 4 = 5$, </li><li> $[2,7]$, $2 \oplus 7 = 5$, </li><li> $[5]$, $5 = 5$, </li><li> $[3,6,8,9,10,11]$, $3 \oplus 6 \oplus 8 \oplus 9 \oplus 10 \oplus 11 = 5$. </li></ul>
