## Description

<div><p>You are given a string $s$ consisting only of characters <span class="tex-font-style-tt">+</span> and <span class="tex-font-style-tt">-</span>. You perform some process with this string. This process can be described by the following pseudocode: </p><pre class="lstlisting"><code class="prettyprint">res = 0<br>for init = 0 to inf<br>    cur = init<br>    ok = true<br>    for i = 1 to |s|<br>        res = res + 1<br>        if s[i] == '+'<br>            cur = cur + 1<br>        else<br>            cur = cur - 1<br>        if cur &lt; 0<br>            ok = false<br>            break<br>    if ok<br>        break<br></code></pre><p>Note that the $inf$ denotes infinity, and the characters of the string are numbered from $1$ to $|s|$.</p><p>You have to calculate the value of the $res$ after the process ends.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>The only lines of each test case contains string $s$ ($1 \le |s| \le 10^6$) consisting only of characters <span class="tex-font-style-tt">+</span> and <span class="tex-font-style-tt">-</span>.</p><p>It's guaranteed that sum of $|s|$ over all test cases doesn't exceed $10^6$.</p></div><div class="output-specification"><p>For each test case print one integer — the value of the $res$ after the process ends.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>The only lines of each test case contains string $s$ ($1 \le |s| \le 10^6$) consisting only of characters <span class="tex-font-style-tt">+</span> and <span class="tex-font-style-tt">-</span>.</p><p>It's guaranteed that sum of $|s|$ over all test cases doesn't exceed $10^6$.</p>

## Output

<p>For each test case print one integer — the value of the $res$ after the process ends.</p>





```input1
3
--+-
---
++--+-
```




```output1
7
9
6
```


