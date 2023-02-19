## Description

<div><p>Let's call a binary string $T$ of length $m$ indexed from $1$ to $m$ <span class="tex-font-style-bf">paranoid</span> if we can obtain a string of length $1$ by performing the following two kinds of operations $m-1$ times in any order :</p><ul><li> Select any substring of $T$ that is equal to <span class="tex-font-style-tt">01</span>, and then replace it with <span class="tex-font-style-tt">1</span>.</li><li> Select any substring of $T$ that is equal to <span class="tex-font-style-tt">10</span>, and then replace it with <span class="tex-font-style-tt">0</span>.<p>For example, if $T = $ <span class="tex-font-style-tt">001</span>, we can select the substring $[T_2T_3]$ and perform the first operation. So we obtain $T = $ <span class="tex-font-style-tt">01</span>.</p></li></ul><p>You are given a binary string $S$ of length $n$ indexed from $1$ to $n$. Find the number of pairs of integers $(l, r)$ $1 \le l \le r \le n$ such that $S[l \ldots r]$ (the substring of $S$ from $l$ to $r$) is a <span class="tex-font-style-bf">paranoid</span> string. </p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of $S$.</p><p>The second line of each test case contains a binary string $S$ of $n$ characters $S_1S_2 \ldots S_n$. ($S_i = $ <span class="tex-font-style-tt">0</span> or $S_i = $ <span class="tex-font-style-tt">1</span> for each $1 \le i \le n$)</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the number of pairs of integers $(l, r)$ $1 \le l \le r \le n$ such that $S[l \ldots r]$ (the substring of $S$ from $l$ to $r$) is a <span class="tex-font-style-bf">paranoid</span> string. </p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of $S$.</p><p>The second line of each test case contains a binary string $S$ of $n$ characters $S_1S_2 \ldots S_n$. ($S_i = $ <span class="tex-font-style-tt">0</span> or $S_i = $ <span class="tex-font-style-tt">1</span> for each $1 \le i \le n$)</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the number of pairs of integers $(l, r)$ $1 \le l \le r \le n$ such that $S[l \ldots r]$ (the substring of $S$ from $l$ to $r$) is a <span class="tex-font-style-bf">paranoid</span> string. </p>





```input1|2,3,6,7,10,11
5
1
1
2
01
3
100
4
1001
5
11111
```




```output1
1
3
4
8
5
```



## Note

<p>In the first sample, $S$ already has length $1$ and doesn't need any operations.</p><p>In the second sample, all substrings of $S$ are <span class="tex-font-style-bf">paranoid</span>. For the entire string, it's enough to perform the first operation.</p><p>In the third sample, all substrings of $S$ are <span class="tex-font-style-bf">paranoid</span> except $[S_2S_3]$, because we can't perform any operations on it, and $[S_1S_2S_3]$ (the entire string).</p>
