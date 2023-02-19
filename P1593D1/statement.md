## Description

<div><p><span class="tex-font-style-it">This problem is a simplified version of D2, but it has significant differences, so read the whole statement.</span></p><p>Polycarp has an array of $n$ ($n$ is even) integers $a_1, a_2, \dots, a_n$. Polycarp conceived of a positive integer $k$. After that, Polycarp began performing the following operations on the array: take an index $i$ ($1 \le i \le n$) and reduce the number $a_i$ by $k$.</p><p>After Polycarp performed some (possibly zero) number of such operations, it turned out that <span class="tex-font-style-bf">all</span> numbers in the array became the same. Find the maximum $k$ at which such a situation is possible, or print $-1$ if such a number can be arbitrarily large.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines. The first line contains an even integer $n$ ($4 \le n \le 40$) ($n$ is even). The second line contains $n$ integers $a_1, a_2, \dots a_n$ ($-10^6 \le a_i \le 10^6$).</p><p>It is guaranteed that the sum of all $n$ specified in the given test cases does not exceed $100$.</p></div><div class="output-specification"><p>For each test case output on a separate line an integer $k$ ($k \ge 1$) — the maximum possible number that Polycarp used in operations on the array, or $-1$, if such a number can be arbitrarily large.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines. The first line contains an even integer $n$ ($4 \le n \le 40$) ($n$ is even). The second line contains $n$ integers $a_1, a_2, \dots a_n$ ($-10^6 \le a_i \le 10^6$).</p><p>It is guaranteed that the sum of all $n$ specified in the given test cases does not exceed $100$.</p>

## Output

<p>For each test case output on a separate line an integer $k$ ($k \ge 1$) — the maximum possible number that Polycarp used in operations on the array, or $-1$, if such a number can be arbitrarily large.</p>





```input1
3
6
1 5 3 1 1 5
8
-1 0 1 -1 0 1 -1 0
4
100 -1000 -1000 -1000
```




```output1
2
1
1100
```


