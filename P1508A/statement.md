## Description

<div><p>A bitstring is a string that contains only the characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>Koyomi Kanou is working hard towards her dream of becoming a writer. To practice, she decided to participate in the <span class="tex-font-style-it">Binary Novel Writing Contest</span>. The writing prompt for the contest consists of three bitstrings of length $2n$. A valid novel for the contest is a bitstring of length at most $3n$ that contains <span class="tex-font-style-bf">at least two</span> of the three given strings as subsequences.</p><p>Koyomi has just received the three prompt strings from the contest organizers. Help her write a valid novel for the contest.</p><p>A string $a$ is a subsequence of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero) characters.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>Each of the following three lines contains a bitstring of length $2n$. It is guaranteed that these three strings are pairwise distinct.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line containing a bitstring of length at most $3n$ that has at least two of the given bitstrings as subsequences.</p><p>It can be proven that under the constraints of the problem, such a bitstring always exists.</p><p>If there are multiple possible answers, you may output any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>Each of the following three lines contains a bitstring of length $2n$. It is guaranteed that these three strings are pairwise distinct.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single line containing a bitstring of length at most $3n$ that has at least two of the given bitstrings as subsequences.</p><p>It can be proven that under the constraints of the problem, such a bitstring always exists.</p><p>If there are multiple possible answers, you may output any of them.</p>





```input1
2
1
00
11
01
3
011001
111010
010001
```




```output1
010
011001010
```



## Note

<p>In the first test case, the bitstrings <span class="tex-font-style-tt">00</span> and <span class="tex-font-style-tt">01</span> are subsequences of the output string: <span class="tex-font-style-tt"><span class="tex-font-style-bf">0</span>1<span class="tex-font-style-bf">0</span></span> and <span class="tex-font-style-tt"><span class="tex-font-style-bf">01</span>0</span>. Note that <span class="tex-font-style-tt">11</span> is not a subsequence of the output string, but this is not required.</p><p>In the second test case all three input strings are subsequences of the output string: <span class="tex-font-style-tt"><span class="tex-font-style-bf">011</span>0<span class="tex-font-style-bf">0</span>1<span class="tex-font-style-bf">01</span>0</span>, <span class="tex-font-style-tt">0<span class="tex-font-style-bf">11</span>00<span class="tex-font-style-bf">1010</span></span> and <span class="tex-font-style-tt"><span class="tex-font-style-bf">0</span>1<span class="tex-font-style-bf">100</span>1<span class="tex-font-style-bf">01</span>0</span>.</p>
