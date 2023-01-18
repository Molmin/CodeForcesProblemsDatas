## Description

<div><p>Recently Polycarp noticed that some of the buttons of his keyboard are malfunctioning. For simplicity, we assume that Polycarp's keyboard contains $26$ buttons (one for each letter of the Latin alphabet). Each button is either working fine or malfunctioning. </p><p>To check which buttons need replacement, Polycarp pressed some buttons in sequence, and a string $s$ appeared on the screen. When Polycarp presses a button with character $c$, one of the following events happened:</p><ul> <li> if the button was working correctly, a character $c$ appeared at the end of the string Polycarp was typing; </li><li> if the button was malfunctioning, <span class="tex-font-style-bf">two</span> characters $c$ appeared at the end of the string. </li></ul><p>For example, suppose the buttons corresponding to characters <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">c</span> are working correctly, and the button corresponding to <span class="tex-font-style-tt">b</span> is malfunctioning. If Polycarp presses the buttons in the order <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">c</span>, <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">b</span>, <span class="tex-font-style-tt">a</span>, then the string he is typing changes as follows: <span class="tex-font-style-tt">a</span> $\rightarrow$ <span class="tex-font-style-tt">abb</span> $\rightarrow$ <span class="tex-font-style-tt">abba</span> $\rightarrow$ <span class="tex-font-style-tt">abbac</span> $\rightarrow$ <span class="tex-font-style-tt">abbaca</span> $\rightarrow$ <span class="tex-font-style-tt">abbacabb</span> $\rightarrow$ <span class="tex-font-style-tt">abbacabba</span>.</p><p>You are given a string $s$ which appeared on the screen after Polycarp pressed some buttons. Help Polycarp to determine which buttons are working correctly for sure (that is, this string could not appear on the screen if any of these buttons was malfunctioning).</p><p>You may assume that the buttons don't start malfunctioning when Polycarp types the string: each button either works correctly throughout the whole process, or malfunctions throughout the whole process.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases in the input.</p><p>Then the test cases follow. Each test case is represented by one line containing a string $s$ consisting of no less than $1$ and no more than $500$ lowercase Latin letters.</p></div><div class="output-specification"><p>For each test case, print one line containing a string $res$. The string $res$ should contain all characters which correspond to buttons that work correctly <span class="tex-font-style-bf">in alphabetical order, without any separators or repetitions</span>. If all buttons may malfunction, $res$ should be empty.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases in the input.</p><p>Then the test cases follow. Each test case is represented by one line containing a string $s$ consisting of no less than $1$ and no more than $500$ lowercase Latin letters.</p>

## Output

<p>For each test case, print one line containing a string $res$. The string $res$ should contain all characters which correspond to buttons that work correctly <span class="tex-font-style-bf">in alphabetical order, without any separators or repetitions</span>. If all buttons may malfunction, $res$ should be empty.</p>





```input1
4
a
zzaaz
ccff
cbddbb
```




```output1
a
z

bc
```


