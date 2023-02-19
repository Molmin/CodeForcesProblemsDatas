## Description

<div><p>You have two binary strings $a$ and $b$ of length $n$. You would like to make all the elements of both strings equal to $0$. Unfortunately, you can modify the contents of these strings using only the following operation:</p><ul> <li> You choose two indices $l$ and $r$ ($1 \le l \le r \le n$); </li><li> For every $i$ that respects $l \le i \le r$, change $a_i$ to the opposite. That is, $a_i := 1 - a_i$; </li><li> For every $i$ that respects either $1 \le i &lt; l$ or $r &lt; i \le n$, change $b_i$ to the opposite. That is, $b_i := 1 - b_i$. </li></ul><p>Your task is to determine if this is possible, and if it is, to find such an appropriate chain of operations. The number of operations <span class="tex-font-style-bf">should not exceed</span> $n + 5$. It can be proven that if such chain of operations exists, one exists with at most $n + 5$ operations. </p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the strings.</p><p>The second line of each test case contains a binary string $a$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, of length $n$.</p><p>The third line of each test case contains a binary string $b$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, of length $n$.</p><p>It is guaranteed that sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print first "<span class="tex-font-style-tt">YES</span>" if it's possible to make all the elements of both strings equal to $0$. Otherwise, print "<span class="tex-font-style-tt">NO</span>". If the answer is "<span class="tex-font-style-tt">YES</span>", on the next line print a single integer $k$ ($0 \le k \le n + 5$) — the number of operations. Then $k$ lines follows, each contains two integers $l$ and $r$ ($1 \le l \le r \le n$) — the description of the operation.</p><p>If there are several correct answers, print any of them.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the strings.</p><p>The second line of each test case contains a binary string $a$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, of length $n$.</p><p>The third line of each test case contains a binary string $b$, consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>, of length $n$.</p><p>It is guaranteed that sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print first "<span class="tex-font-style-tt">YES</span>" if it's possible to make all the elements of both strings equal to $0$. Otherwise, print "<span class="tex-font-style-tt">NO</span>". If the answer is "<span class="tex-font-style-tt">YES</span>", on the next line print a single integer $k$ ($0 \le k \le n + 5$) — the number of operations. Then $k$ lines follows, each contains two integers $l$ and $r$ ($1 \le l \le r \le n$) — the description of the operation.</p><p>If there are several correct answers, print any of them.</p>





```input1|2,3,4,8,9,10,14,15,16
5
3
010
101
2
11
10
4
1000
0011
2
10
10
3
111
111
```




```output1
YES
1
2 2
NO
NO
YES
2
1 2
2 2
YES
2
1 1
2 3
```



## Note

<p>In the first test case, we can perform one operation with $l = 2$ and $r = 2$. So $a_2 := 1 - 1 = 0$ and string $a$ became equal to <span class="tex-font-style-tt">000</span>. $b_1 := 1 - 1 = 0$, $b_3 := 1 - 1 = 0$ and string $b$ became equal to <span class="tex-font-style-tt">000</span>.</p><p>In the second and in the third test cases, it can be proven that it's impossible to make all elements of both strings equal to $0$.</p><p>In the fourth test case, we can perform an operation with $l = 1$ and $r = 2$, then string $a$ became equal to <span class="tex-font-style-tt">01</span>, and string $b$ doesn't change. Then we perform an operation with $l = 2$ and $r = 2$, then $a_2 := 1 - 1 = 0$ and $b_1 = 1 - 1 = 0$. So both of string $a$ and $b$ became equal to <span class="tex-font-style-tt">00</span>.</p><p>In the fifth test case, we can perform an operation with $l = 1$ and $r = 1$. Then string $a$ became equal to <span class="tex-font-style-tt">011</span> and string $b$ became equal to <span class="tex-font-style-tt">100</span>. Then we can perform an operation with $l = 2$ and $r = 3$, so both of string $a$ and $b$ became equal to <span class="tex-font-style-tt">000</span>.</p>
