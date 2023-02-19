## Description

<div><p>You are given two strings $s$ and $t$, both of length $n$. Each character in both string is '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' or '<span class="tex-font-style-tt">c</span>'.</p><p>In one move, you can perform one of the following actions: </p><ul> <li> choose an occurrence of "<span class="tex-font-style-tt">ab</span>" in $s$ and replace it with "<span class="tex-font-style-tt">ba</span>"; </li><li> choose an occurrence of "<span class="tex-font-style-tt">bc</span>" in $s$ and replace it with "<span class="tex-font-style-tt">cb</span>". </li></ul><p>You are allowed to perform an arbitrary amount of moves (possibly, zero). Can you change string $s$ to make it equal to string $t$?</p></div><div class="input-specification"><p>The first line contains a single integer $q$ ($1 \le q \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of strings $s$ and $t$.</p><p>The second line contains string $s$ of length $n$. Each character is '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' or '<span class="tex-font-style-tt">c</span>'.</p><p>The third line contains string $t$ of length $n$. Each character is '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' or '<span class="tex-font-style-tt">c</span>'.</p><p>The sum of $n$ over all testcases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if you can change string $s$ to make it equal to string $t$ by performing an arbitrary amount of moves (possibly, zero). Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $q$ ($1 \le q \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of strings $s$ and $t$.</p><p>The second line contains string $s$ of length $n$. Each character is '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' or '<span class="tex-font-style-tt">c</span>'.</p><p>The third line contains string $t$ of length $n$. Each character is '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' or '<span class="tex-font-style-tt">c</span>'.</p><p>The sum of $n$ over all testcases doesn't exceed $10^5$.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if you can change string $s$ to make it equal to string $t$ by performing an arbitrary amount of moves (possibly, zero). Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
5
3
cab
cab
1
a
b
6
abbabc
bbaacb
10
bcaabababc
cbbababaac
2
ba
ab
```




```output1
YES
NO
YES
YES
NO
```


