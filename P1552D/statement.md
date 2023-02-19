## Description

<div><p>You are given a sequence of $n$ integers $a_1, \, a_2, \, \dots, \, a_n$.</p><p>Does there exist a sequence of $n$ integers $b_1, \, b_2, \, \dots, \, b_n$ such that the following property holds?</p><ul> <li> For each $1 \le i \le n$, there exist two (not necessarily distinct) indices $j$ and $k$ ($1 \le j, \, k \le n$) such that $a_i = b_j - b_k$. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 20$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10$).</p><p>The second line of each test case contains the $n$ integers $a_1, \, \dots, \, a_n$ ($-10^5 \le a_i \le 10^5$).</p></div><div class="output-specification"><p>For each test case, output a line containing <span class="tex-font-style-tt">YES</span> if a sequence $b_1, \, \dots, \, b_n$ satisfying the required property exists, and <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 20$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 10$).</p><p>The second line of each test case contains the $n$ integers $a_1, \, \dots, \, a_n$ ($-10^5 \le a_i \le 10^5$).</p>

## Output

<p>For each test case, output a line containing <span class="tex-font-style-tt">YES</span> if a sequence $b_1, \, \dots, \, b_n$ satisfying the required property exists, and <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
5
5
4 -7 -1 5 10
1
0
3
1 10 100
4
-3 2 10 2
9
25 -171 250 174 152 242 100 -205 -258
```




```output1
YES
YES
NO
YES
YES
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, the sequence $b = [-9, \, 2, \, 1, \, 3, \, -2]$ satisfies the property. Indeed, the following holds: </p><ul> <li> $a_1 = 4 = 2 - (-2) = b_2 - b_5$; </li><li> $a_2 = -7 = -9 - (-2) = b_1 - b_5$; </li><li> $a_3 = -1 = 1 - 2 = b_3 - b_2$; </li><li> $a_4 = 5 = 3 - (-2) = b_4 - b_5$; </li><li> $a_5 = 10 = 1 - (-9) = b_3 - b_1$. </li></ul><p>In the <span class="tex-font-style-bf">second test case</span>, it is sufficient to choose $b = [0]$, since $a_1 = 0 = 0 - 0 = b_1 - b_1$.</p><p>In the <span class="tex-font-style-bf">third test case</span>, it is possible to show that no sequence $b$ of length $3$ satisfies the property.</p>
