## Description

<div><p>For an array of <span class="tex-font-style-bf">non-negative</span> integers $a$ of size $n$, we construct another array $d$ as follows: $d_1 = a_1$, $d_i = |a_i - a_{i - 1}|$ for $2 \le i \le n$.</p><p>Your task is to restore the array $a$ from a given array $d$, or to report that there are multiple possible arrays. </p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the size of the arrays $a$ and $d$.</p><p>The second line contains $n$ integers $d_1, d_2, \dots, d_n$ ($0 \le d_i \le 100$)&nbsp;— the elements of the array $d$.</p><p>It can be shown that there always exists at least one suitable array $a$ under these constraints.</p></div><div class="output-specification"><p>For each test case, print the elements of the array $a$, if there is only one possible array $a$. Otherwise, print $-1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 100$)&nbsp;— the size of the arrays $a$ and $d$.</p><p>The second line contains $n$ integers $d_1, d_2, \dots, d_n$ ($0 \le d_i \le 100$)&nbsp;— the elements of the array $d$.</p><p>It can be shown that there always exists at least one suitable array $a$ under these constraints.</p>

## Output

<p>For each test case, print the elements of the array $a$, if there is only one possible array $a$. Otherwise, print $-1$.</p>





```input1|2,3,6,7
3
4
1 0 2 5
3
2 6 3
5
0 0 0 0 0
```




```output1
1 1 3 8
-1
0 0 0 0 0
```



## Note

<p>In the second example, there are two suitable arrays: $[2, 8, 5]$ and $[2, 8, 11]$.</p>
