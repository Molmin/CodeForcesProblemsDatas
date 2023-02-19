## Description

<div><p><span class="tex-font-style-it">Mihai plans to watch a movie. He only likes palindromic movies, so he wants to skip some (possibly zero) scenes to make the remaining parts of the movie palindromic.</span></p><p>You are given a list $s$ of $n$ non-empty strings of length <span class="tex-font-style-bf">at most $3$</span>, representing the scenes of Mihai's movie.</p><p>A subsequence of $s$ is called <span class="tex-font-style-it">awesome</span> if it is non-empty and the concatenation of the strings in the subsequence, in order, is a palindrome.</p><p>Can you help Mihai check if there is at least one awesome subsequence of $s$?</p><p>A palindrome is a string that reads the same backward as forward, for example strings "<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">aba</span>", "<span class="tex-font-style-tt">abccba</span>" are palindromes, but strings "<span class="tex-font-style-tt">codeforces</span>", "<span class="tex-font-style-tt">reality</span>", "<span class="tex-font-style-tt">ab</span>" are not.</p><p>A sequence $a$ is a non-empty subsequence of a non-empty sequence $b$ if $a$ can be obtained from $b$ by deletion of several (possibly zero, but not all) elements.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the number of scenes in the movie.</p><p>Then follows $n$ lines, the $i$-th of which containing a single non-empty string $s_i$ of length at most $3$, consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if there is an awesome subsequence of $s$, or "<span class="tex-font-style-tt">NO</span>" otherwise (case insensitive).</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the number of scenes in the movie.</p><p>Then follows $n$ lines, the $i$-th of which containing a single non-empty string $s_i$ of length at most $3$, consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if there is an awesome subsequence of $s$, or "<span class="tex-font-style-tt">NO</span>" otherwise (case insensitive).</p>





```input1
6
5
zx
ab
cc
zx
ba
2
ab
bad
4
co
def
orc
es
3
a
b
c
3
ab
cd
cba
2
ab
ab
```




```output1
YES
NO
NO
YES
YES
NO
```



## Note

<p>In the first test case, an awesome subsequence of $s$ is $[ab, cc, ba]$</p>
