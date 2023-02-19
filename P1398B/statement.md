## Description

<div><p>Alice and Bob play a game. They have a binary string $s$ (a string such that each character in it is either $0$ or $1$). Alice moves first, then Bob, then Alice again, and so on.</p><p>During their move, the player can choose any number (not less than one) of <span class="tex-font-style-bf">consecutive equal characters</span> in $s$ and delete them.</p><p>For example, if the string is $10110$, there are $6$ possible moves (deleted characters are bold):</p><ol> <li> $\textbf{1}0110 \to 0110$; </li><li> $1\textbf{0}110 \to 1110$; </li><li> $10\textbf{1}10 \to 1010$; </li><li> $101\textbf{1}0 \to 1010$; </li><li> $10\textbf{11}0 \to 100$; </li><li> $1011\textbf{0} \to 1011$. </li></ol><p>After the characters are removed, the characters to the left and to the right of the removed block become adjacent. I. e. the following sequence of moves is valid: $10\textbf{11}0 \to 1\textbf{00} \to 1$.</p><p>The game ends when the string becomes empty, and the score of each player is <span class="tex-font-style-bf">the number of $1$-characters deleted by them</span>.</p><p>Each player wants to maximize their score. Calculate the resulting score of Alice.</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 500$) — the number of test cases.</p><p>Each test case contains exactly one line containing a binary string $s$ ($1 \le |s| \le 100$).</p></div><div class="output-specification"><p>For each test case, print one integer — the resulting score of Alice (the number of $1$-characters deleted by her).</p></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 500$) — the number of test cases.</p><p>Each test case contains exactly one line containing a binary string $s$ ($1 \le |s| \le 100$).</p>

## Output

<p>For each test case, print one integer — the resulting score of Alice (the number of $1$-characters deleted by her).</p>





```input1
5
01111001
0000
111111
101010101
011011110111
```




```output1
4
0
6
3
6
```



## Note

<p>Questions about the optimal strategy will be ignored.</p>
