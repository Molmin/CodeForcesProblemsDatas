## Description

<div><p>A <span class="tex-font-style-it">palindrome</span> is a string that reads the same backward as forward. For example, the strings $\texttt{z}$, $\texttt{aaa}$, $\texttt{aba}$, and $\texttt{abccba}$ are palindromes, but $\texttt{codeforces}$ and $\texttt{ab}$ are not.</p><p>The <span class="tex-font-style-it">double</span> of a string $s$ is obtained by writing each character twice. For example, the double of $\texttt{seeing}$ is $\texttt{sseeeeiinngg}$.</p><p>Given a string $s$, rearrange its double to form a palindrome. Output the rearranged string. It can be proven that such a rearrangement always exists.</p></div><div class="input-specification"><p>The first line of input contains $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains a single string $s$ ($1 \leq |s| \leq 100$) consisting only of lowercase English letters.</p><p>Note that the sum of $|s|$ over all test cases is not bounded.</p></div><div class="output-specification"><p>For each test case, output a palindromic string of length $2 \cdot |s|$ that is a rearrangement of the double of $s$.</p></div>

## Input

<p>The first line of input contains $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains a single string $s$ ($1 \leq |s| \leq 100$) consisting only of lowercase English letters.</p><p>Note that the sum of $|s|$ over all test cases is not bounded.</p>

## Output

<p>For each test case, output a palindromic string of length $2 \cdot |s|$ that is a rearrangement of the double of $s$.</p>





```input1|2,4
4
a
sururu
errorgorn
anutforajaroftuna
```




```output1
aa
suurruurruus
rgnororerrerorongr
aannuuttffoorraajjaarrooffttuunnaa
```



## Note

<p>In the first test case, the double of $\texttt{a}$ is $\texttt{aa}$, which is already a palindrome.</p><p>In the second test case, the double of $\texttt{sururu}$ is $\texttt{ssuurruurruu}$. If we move the first $\texttt{s}$ to the end, we get $\texttt{suurruurruus}$, which is a palindrome.</p><p>In the third test case, the double of $\texttt{errorgorn}$ is $\texttt{eerrrroorrggoorrnn}$. We can rearrange the characters to form $\texttt{rgnororerrerorongr}$, which is a palindrome.</p>
