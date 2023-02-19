## Description

<div><p>You are given a string $s$. You need to find two non-empty strings $a$ and $b$ such that the following conditions are satisfied:</p><ol> <li> Strings $a$ and $b$ are both <span class="tex-font-style-bf">subsequences</span> of $s$. </li><li> For each index $i$, character $s_i$ of string $s$ must belong to <span class="tex-font-style-bf">exactly one</span> of strings $a$ or $b$. </li><li> String $a$ is <span class="tex-font-style-it">lexicographically</span> minimum possible; string $b$ may be any possible string. </li></ol><p>Given string $s$, print any valid $a$ and $b$.</p><p><span class="tex-font-style-bf">Reminder:</span></p><p>A string $a$ ($b$) is a <span class="tex-font-style-it">subsequence</span> of a string $s$ if $a$ ($b$) can be obtained from $s$ by deletion of several (possibly, zero) elements. For example, "<span class="tex-font-style-tt">dores</span>", "<span class="tex-font-style-tt">cf</span>", and "<span class="tex-font-style-tt">for</span>" are subsequences of "<span class="tex-font-style-tt">codeforces</span>", while "<span class="tex-font-style-tt">decor</span>" and "<span class="tex-font-style-tt">fork</span>" are not.</p><p>A string $x$ is <span class="tex-font-style-it">lexicographically smaller</span> than a string $y$ if and only if one of the following holds:</p><ul> <li> $x$ is a prefix of $y$, but $x \ne y$; </li><li> in the first position where $x$ and $y$ differ, the string $x$ has a letter that appears earlier in the alphabet than the corresponding letter in $y$. </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first and only line of each test case contains one string $s$ ($2 \le |s| \le 100$ where $|s|$ means the length of $s$). String $s$ consists of lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, print the strings $a$ and $b$ that satisfy the given conditions. If there are multiple answers, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first and only line of each test case contains one string $s$ ($2 \le |s| \le 100$ where $|s|$ means the length of $s$). String $s$ consists of lowercase Latin letters.</p>

## Output

<p>For each test case, print the strings $a$ and $b$ that satisfy the given conditions. If there are multiple answers, print any.</p>





```input1
3
fc
aaaa
thebrightboiler
```




```output1
c f
a aaa
b therightboiler
```



## Note

<p>In the first test case, there are only two choices: either $a =$ <span class="tex-font-style-tt">f</span> and $b = $ <span class="tex-font-style-tt">c</span> or $a = $ <span class="tex-font-style-tt">c</span> and $b = $ <span class="tex-font-style-tt">f</span>. And $a = $<span class="tex-font-style-tt">c</span> is lexicographically smaller than $a = $ <span class="tex-font-style-tt">f</span>.</p><p>In the second test case, <span class="tex-font-style-tt">a</span> is the only character in the string.</p><p>In the third test case, it can be proven that <span class="tex-font-style-tt">b</span> is the lexicographically smallest subsequence of $s$. The second string can be of two variants; one of them is given here.</p>
