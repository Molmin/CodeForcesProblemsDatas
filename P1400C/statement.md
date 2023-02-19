## Description

<div><p>Consider the following process. You have a binary string (a string where each character is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>) $w$ of length $n$ and an integer $x$. You build a new binary string $s$ consisting of $n$ characters. The $i$-th character of $s$ is chosen as follows:</p><ul> <li> if the character $w_{i-x}$ exists and is equal to <span class="tex-font-style-tt">1</span>, then $s_i$ is <span class="tex-font-style-tt">1</span> (formally, if $i &gt; x$ and $w_{i-x} = $ <span class="tex-font-style-tt">1</span>, then $s_i = $ <span class="tex-font-style-tt">1</span>); </li><li> if the character $w_{i+x}$ exists and is equal to <span class="tex-font-style-tt">1</span>, then $s_i$ is <span class="tex-font-style-tt">1</span> (formally, if $i + x \le n$ and $w_{i+x} = $ <span class="tex-font-style-tt">1</span>, then $s_i = $ <span class="tex-font-style-tt">1</span>); </li><li> if both of the aforementioned conditions are false, then $s_i$ is <span class="tex-font-style-tt">0</span>. </li></ul><p>You are given the integer $x$ and the resulting string $s$. Reconstruct the original string $w$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains the resulting string $s$ ($2 \le |s| \le 10^5$, each character of $s$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>). The second line contains one integer $x$ ($1 \le x \le |s| - 1$).</p><p>The total length of all strings $s$ in the input does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the answer on a separate line as follows:</p><ul> <li> if no string $w$ can produce the string $s$ at the end of the process, print $-1$; </li><li> otherwise, print the binary string $w$ consisting of $|s|$ characters. If there are multiple answers, print any of them. </li></ul></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases.</p><p>Each test case consists of two lines. The first line contains the resulting string $s$ ($2 \le |s| \le 10^5$, each character of $s$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>). The second line contains one integer $x$ ($1 \le x \le |s| - 1$).</p><p>The total length of all strings $s$ in the input does not exceed $10^5$.</p>

## Output

<p>For each test case, print the answer on a separate line as follows:</p><ul> <li> if no string $w$ can produce the string $s$ at the end of the process, print $-1$; </li><li> otherwise, print the binary string $w$ consisting of $|s|$ characters. If there are multiple answers, print any of them. </li></ul>





```input1
3
101110
2
01
1
110
1
```




```output1
111011
10
-1
```


