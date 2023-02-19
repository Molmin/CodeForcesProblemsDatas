## Description

<div><p>A binary string is a string where each character is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>. Two binary strings $a$ and $b$ of equal length are <span class="tex-font-style-it">similar</span>, if they have the same character in some position (there exists an integer $i$ such that $a_i = b_i$). For example:</p><ul> <li> <span class="tex-font-style-tt">10010</span> and <span class="tex-font-style-tt">01111</span> are <span class="tex-font-style-it">similar</span> (they have the same character in position $4$); </li><li> <span class="tex-font-style-tt">10010</span> and <span class="tex-font-style-tt">11111</span> are <span class="tex-font-style-it">similar</span>; </li><li> <span class="tex-font-style-tt">111</span> and <span class="tex-font-style-tt">111</span> are <span class="tex-font-style-it">similar</span>; </li><li> <span class="tex-font-style-tt">0110</span> and <span class="tex-font-style-tt">1001</span> are not <span class="tex-font-style-it">similar</span>. </li></ul><p>You are given an integer $n$ and a binary string $s$ consisting of $2n-1$ characters. Let's denote $s[l..r]$ as the contiguous substring of $s$ starting with $l$-th character and ending with $r$-th character (in other words, $s[l..r] = s_l s_{l + 1} s_{l + 2} \dots s_r$).</p><p>You have to construct a binary string $w$ of length $n$ which is <span class="tex-font-style-it">similar</span> to <span class="tex-font-style-bf">all of the following strings</span>: $s[1..n]$, $s[2..n+1]$, $s[3..n+2]$, ..., $s[n..2n-1]$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$).</p><p>The second line of each test case contains the binary string $s$ of length $2n - 1$. Each character $s_i$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>For each test case, print the corresponding binary string $w$ of length $n$. If there are multiple such strings — print any of them. It can be shown that at least one string $w$ meeting the constraints always exists.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$).</p><p>The second line of each test case contains the binary string $s$ of length $2n - 1$. Each character $s_i$ is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>For each test case, print the corresponding binary string $w$ of length $n$. If there are multiple such strings — print any of them. It can be shown that at least one string $w$ meeting the constraints always exists.</p>





```input1
4
1
1
3
00000
4
1110000
2
101
```




```output1
1
000
1010
00
```



## Note

<p>The explanation of the sample case (equal characters in equal positions are bold):</p><p>The first test case: </p><ul> <li> $\mathbf{1}$ is similar to $s[1..1] = \mathbf{1}$. </li></ul><p>The second test case: </p><ul> <li> $\mathbf{000}$ is similar to $s[1..3] = \mathbf{000}$; </li><li> $\mathbf{000}$ is similar to $s[2..4] = \mathbf{000}$; </li><li> $\mathbf{000}$ is similar to $s[3..5] = \mathbf{000}$. </li></ul><p>The third test case: </p><ul> <li> $\mathbf{1}0\mathbf{10}$ is similar to $s[1..4] = \mathbf{1}1\mathbf{10}$; </li><li> $\mathbf{1}01\mathbf{0}$ is similar to $s[2..5] = \mathbf{1}10\mathbf{0}$; </li><li> $\mathbf{10}1\mathbf{0}$ is similar to $s[3..6] = \mathbf{10}0\mathbf{0}$; </li><li> $1\mathbf{0}1\mathbf{0}$ is similar to $s[4..7] = 0\mathbf{0}0\mathbf{0}$. </li></ul><p>The fourth test case: </p><ul> <li> $0\mathbf{0}$ is similar to $s[1..2] = 1\mathbf{0}$; </li><li> $\mathbf{0}0$ is similar to $s[2..3] = \mathbf{0}1$. </li></ul>
