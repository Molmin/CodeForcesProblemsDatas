## Description

<div><p>For some binary string $s$ (i.e. each character $s_i$ is either '<span class="tex-font-style-tt">0</span>' or '<span class="tex-font-style-tt">1</span>'), all pairs of consecutive (adjacent) characters were written. In other words, all substrings of length $2$ were written. For each pair (substring of length $2$), the number of '<span class="tex-font-style-tt">1</span>' (ones) in it was calculated.</p><p>You are given three numbers:</p><ul> <li> $n_0$ — the number of such pairs of consecutive characters (substrings) where the number of ones equals $0$; </li><li> $n_1$ — the number of such pairs of consecutive characters (substrings) where the number of ones equals $1$; </li><li> $n_2$ — the number of such pairs of consecutive characters (substrings) where the number of ones equals $2$. </li></ul><p>For example, for the string $s=$"<span class="tex-font-style-tt">1110011110</span>", the following substrings would be written: "<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">00</span>", "<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">10</span>". Thus, $n_0=1$, $n_1=3$, $n_2=5$.</p><p>Your task is to restore <span class="tex-font-style-bf">any</span> suitable binary string $s$ from the given values $n_0, n_1, n_2$. It is guaranteed that at least one of the numbers $n_0, n_1, n_2$ is greater than $0$. Also, it is guaranteed that a solution exists.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$) — the number of test cases in the input. Then test cases follow.</p><p>Each test case consists of one line which contains three integers $n_0, n_1, n_2$ ($0 \le n_0, n_1, n_2 \le 100$; $n_0 + n_1 + n_2 &gt; 0$). It is guaranteed that the answer for given $n_0, n_1, n_2$ exists.</p></div><div class="output-specification"><p>Print $t$ lines. Each of the lines should contain a binary string corresponding to a test case. If there are several possible solutions, print any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$) — the number of test cases in the input. Then test cases follow.</p><p>Each test case consists of one line which contains three integers $n_0, n_1, n_2$ ($0 \le n_0, n_1, n_2 \le 100$; $n_0 + n_1 + n_2 &gt; 0$). It is guaranteed that the answer for given $n_0, n_1, n_2$ exists.</p>

## Output

<p>Print $t$ lines. Each of the lines should contain a binary string corresponding to a test case. If there are several possible solutions, print any of them.</p>





```input1
7
1 3 5
1 1 1
3 9 3
0 1 0
3 1 2
0 0 3
2 0 0
```




```output1
1110011110
0011
0110001100101011
10
0000111
1111
000
```


