## Description

<div><p>You are given two arrays $a$ and $b$, both consisting of $n$ integers.</p><p>In one move, you can choose two indices $i$ and $j$ ($1 \le i, j \le n$; $i \neq j$) and swap $a_i$ with $a_j$ and $b_i$ with $b_j$. You have to perform the swap in both arrays.</p><p>You are allowed to perform at most $10^4$ moves (possibly, zero). Can you make both arrays sorted in a non-decreasing order at the end? If you can, print any sequence of moves that makes both arrays sorted.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the number of elements in both arrays.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the first array.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$)&nbsp;— the second array.</p></div><div class="output-specification"><p>For each testcase, print the answer. If it's impossible to make both arrays sorted in a non-decreasing order in at most $10^4$ moves, print <span class="tex-font-style-tt">-1</span>. Otherwise, first, print the number of moves $k$ $(0 \le k \le 10^4)$. Then print $i$ and $j$ for each move $(1 \le i, j \le n$; $i \neq j)$.</p><p>If there are multiple answers, then print any of them. You don't have to minimize the number of moves.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the number of elements in both arrays.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the first array.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le n$)&nbsp;— the second array.</p>

## Output

<p>For each testcase, print the answer. If it's impossible to make both arrays sorted in a non-decreasing order in at most $10^4$ moves, print <span class="tex-font-style-tt">-1</span>. Otherwise, first, print the number of moves $k$ $(0 \le k \le 10^4)$. Then print $i$ and $j$ for each move $(1 \le i, j \le n$; $i \neq j)$.</p><p>If there are multiple answers, then print any of them. You don't have to minimize the number of moves.</p>





```input1
3
2
1 2
1 2
2
2 1
1 2
4
2 3 1 2
2 3 2 3
```




```output1
0
-1
3
3 1
3 2
4 3
```


