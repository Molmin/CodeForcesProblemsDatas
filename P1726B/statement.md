## Description

<div><p>Mainak has two positive integers $n$ and $m$.</p><p>Mainak finds a sequence $a_1, a_2, \ldots, a_n$ of $n$ positive integers <span class="tex-font-style-it">interesting</span>, if <span class="tex-font-style-bf">for all</span> integers $i$ ($1 \le i \le n$), the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of all elements in $a$ which are <span class="tex-font-style-bf">strictly less</span> than $a_i$ is $0$. Formally if $p_i$ is the bitwise XOR of all elements in $a$ which are strictly less than $a_i$, then $a$ is an <span class="tex-font-style-it">interesting</span> sequence if $p_1 = p_2 = \ldots = p_n = 0$.</p><p>For example, sequences $[1,3,2,3,1,2,3]$, $[4,4,4,4]$, $[25]$ are <span class="tex-font-style-it">interesting</span>, whereas $[1,2,3,4]$ ($p_2 = 1 \ne 0$), $[4,1,1,2,4]$ ($p_1 = 1 \oplus 1 \oplus 2 = 2 \ne 0$), $[29,30,30]$ ($p_2 = 29 \ne 0$) aren't interesting.</p><p>Here $a \oplus b$ denotes bitwise XOR of integers $a$ and $b$.</p><p>Find any <span class="tex-font-style-it">interesting</span> sequence $a_1, a_2, \ldots, a_n$ (or report that there exists no such sequence) such that the sum of the elements in the sequence $a$ is equal to $m$, i.e. $a_1 + a_2 \ldots + a_n = m$.</p><p>As a reminder, the bitwise XOR of an empty sequence is considered to be $0$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line and the only line of each test case contains two integers $n$ and $m$ ($1 \le n \le 10^5$, $1 \le m \le 10^9$) — the length of the sequence and the sum of the elements.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if there exists some interesting sequence, output "<span class="tex-font-style-tt">Yes</span>" on the first line, otherwise output "<span class="tex-font-style-tt">No</span>". You may print each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>" will all be recognized as positive answer).</p><p>If the answer is "<span class="tex-font-style-tt">Yes</span>", output $n$ <span class="tex-font-style-bf">positive integers</span> $a_1, a_2, \ldots, a_n$ ($a_i \ge 1$), forming an <span class="tex-font-style-it">interesting</span> sequence such that $a_1 + a_2 \ldots + a_n = m$. If there are multiple solutions, output any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line and the only line of each test case contains two integers $n$ and $m$ ($1 \le n \le 10^5$, $1 \le m \le 10^9$) — the length of the sequence and the sum of the elements.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, if there exists some interesting sequence, output "<span class="tex-font-style-tt">Yes</span>" on the first line, otherwise output "<span class="tex-font-style-tt">No</span>". You may print each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>" will all be recognized as positive answer).</p><p>If the answer is "<span class="tex-font-style-tt">Yes</span>", output $n$ <span class="tex-font-style-bf">positive integers</span> $a_1, a_2, \ldots, a_n$ ($a_i \ge 1$), forming an <span class="tex-font-style-it">interesting</span> sequence such that $a_1 + a_2 \ldots + a_n = m$. If there are multiple solutions, output any.</p>





```input1
4
1 3
6 12
2 1
3 6
```




```output1
Yes
3
Yes
1 3 2 2 3 1
No
Yes
2 2 2
```



## Note

<ul><li> In the first test case, $[3]$ is the only interesting sequence of length $1$ having sum $3$.</li><li> In the third test case, there is no sequence of length $2$ having sum of elements equal to $1$, so there is no such interesting sequence.</li><li> In the fourth test case, $p_1 = p_2 = p_3 = 0$, because bitwise XOR of an empty sequence is $0$.</li></ul>
