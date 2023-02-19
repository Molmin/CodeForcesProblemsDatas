## Description

<div><p>Once <span class="tex-font-style-it">Divan</span> analyzed a sequence $a_1, a_2, \ldots, a_n$ consisting of $n$ non-negative integers as follows. He considered each non-empty <span class="tex-font-style-it">subsequence</span> of the sequence $a$, computed the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of its elements and added up all the XORs, obtaining the <span class="tex-font-style-it">coziness</span> of the sequence $a$.</p><p>A sequence $c$ is a <span class="tex-font-style-it">subsequence</span> of a sequence $d$ if $c$ can be obtained from $d$ by deletion of several (possibly, zero or all) elements. For example, $[1, \, 2, \, 3, \, 4]$, $[2, \, 4]$, and $[2]$ are subsequences of $[1, \, 2, \, 3, \, 4]$, but $[4, \, 3]$ and $[0]$ are not.</p><p><span class="tex-font-style-it">Divan</span> was very proud of his analysis, but now he lost the sequence $a$, and also the coziness value! However, <span class="tex-font-style-it">Divan</span> remembers the value of <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> on $m$ contiguous subsegments of the sequence $a$. It turns out that each element of the original sequence is contained in <span class="tex-font-style-bf">at least one</span> of these $m$ segments.</p><p><span class="tex-font-style-it">Divan</span> asks you to help find the coziness of the sequence $a$ using the information he remembers. If several coziness values are possible, print any.</p><p>As the result can be very large, print the value modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains one integer number $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>The first line of each test case contains two integer numbers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the length of the sequence and the number of contiguous segments whose bitwise OR values <span class="tex-font-style-it">Divan</span> remembers, respectively.</p><p>The following $m$ lines describe the segments, one per line.</p><p>Each segment is described with three integers $l$, $r$, and $x$ ($1 \le l \le r \le n$, $0 \le x \le 2^{30} - 1$) — the first and last elements of the segment and the bitwise OR of $a_l, a_{l + 1}, \ldots, a_r$, respectively.</p><p>It is guaranteed that each element of the sequence is contained in at least one of the segments. It is guaranteed that there exists a sequence that satisfies all constraints.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all test cases do not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case print the coziness any suitable sequence $a$ modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains one integer number $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>The first line of each test case contains two integer numbers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the length of the sequence and the number of contiguous segments whose bitwise OR values <span class="tex-font-style-it">Divan</span> remembers, respectively.</p><p>The following $m$ lines describe the segments, one per line.</p><p>Each segment is described with three integers $l$, $r$, and $x$ ($1 \le l \le r \le n$, $0 \le x \le 2^{30} - 1$) — the first and last elements of the segment and the bitwise OR of $a_l, a_{l + 1}, \ldots, a_r$, respectively.</p><p>It is guaranteed that each element of the sequence is contained in at least one of the segments. It is guaranteed that there exists a sequence that satisfies all constraints.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all test cases do not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case print the coziness any suitable sequence $a$ modulo $10^9 + 7$.</p>





```input1
3
2 1
1 2 2
3 2
1 3 5
2 3 5
5 4
1 2 7
3 3 7
4 4 0
4 5 2
```




```output1
4
20
112
```



## Note

<p>In first example, one of the sequences that fits the constraints is $[0, 2]$. Consider all its non-empty subsequences:</p><ul> <li> $[0]$: the bitwise XOR of this subsequence is $0$; </li><li> $[2]$: the bitwise XOR of this subsequence is $2$; </li><li> $[0, 2]$: the bitwise XOR of this subsequence is $2$. </li></ul><p>The sum of all results is $4$, so it is the answer.</p><p>In second example, one of the sequences that fits the constraints is $[0, \, 5, \, 5]$.</p><p>In third example, one of the sequences that fits the constraints is $[5, \, 6, \, 7, \, 0, \, 2]$.</p>
