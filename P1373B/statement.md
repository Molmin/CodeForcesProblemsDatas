## Description

<div><p>Alica and Bob are playing a game.</p><p>Initially they have a binary string $s$ consisting of only characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p><p>Alice and Bob make alternating moves: Alice makes the first move, Bob makes the second move, Alice makes the third one, and so on. During each move, the current player must choose two <span class="tex-font-style-bf">different adjacent</span> characters of string $s$ and delete them. For example, if $s = 1011001$ then the following moves are possible: </p><ol> <li> delete $s_1$ and $s_2$: $\textbf{10}11001 \rightarrow 11001$; </li><li> delete $s_2$ and $s_3$: $1\textbf{01}1001 \rightarrow 11001$; </li><li> delete $s_4$ and $s_5$: $101\textbf{10}01 \rightarrow 10101$; </li><li> delete $s_6$ and $s_7$: $10110\textbf{01} \rightarrow 10110$. </li></ol><p>If a player can't make any move, they lose. Both players play optimally. You have to determine if Alice can win.</p></div><div class="input-specification"><p>First line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Only line of each test case contains one string $s$ ($1 \le |s| \le 100$), consisting of only characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>For each test case print answer in the single line.</p><p>If Alice can win print <span class="tex-font-style-tt">DA</span> (YES in Russian) in any register. Otherwise print <span class="tex-font-style-tt">NET</span> (NO in Russian) in any register.</p></div>

## Input

<p>First line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Only line of each test case contains one string $s$ ($1 \le |s| \le 100$), consisting of only characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>For each test case print answer in the single line.</p><p>If Alice can win print <span class="tex-font-style-tt">DA</span> (YES in Russian) in any register. Otherwise print <span class="tex-font-style-tt">NET</span> (NO in Russian) in any register.</p>





```input1
3
01
1111
0011
```




```output1
DA
NET
NET
```



## Note

<p>In the first test case after Alice's move string $s$ become empty and Bob can not make any move.</p><p>In the second test case Alice can not make any move initially.</p><p>In the third test case after Alice's move string $s$ turn into $01$. Then, after Bob's move string $s$ become empty and Alice can not make any move.</p>
