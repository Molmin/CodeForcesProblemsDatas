## Description

<div><p>Alice and Bob are playing a game with strings. There will be $t$ rounds in the game. In each round, there will be a string $s$ consisting of lowercase English letters. </p><p>Alice moves first and both the players take alternate turns. <span class="tex-font-style-bf">Alice is allowed to remove any substring of even length (possibly empty) and Bob is allowed to remove any substring of odd length from $s$</span>.</p><p>More formally, if there was a string $s = s_1s_2 \ldots s_k$ the player can choose a substring $s_ls_{l+1} \ldots s_{r-1}s_r$ with length of corresponding parity and remove it. After that the string will become $s = s_1 \ldots s_{l-1}s_{r+1} \ldots s_k$.</p><p>After the string becomes empty, the round ends and each player calculates his/her score for this round. The score of a player is the sum of values of all characters removed by him/her. The value of $\texttt{a}$ is $1$, the value of $\texttt{b}$ is $2$, the value of $\texttt{c}$ is $3$, $\ldots$, and the value of $\texttt{z}$ is $26$. The player with higher score wins the round. For each round, determine the winner and the difference between winner's and loser's scores. Assume that both players play optimally to maximize their score. It can be proved that a draw is impossible.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1\leq t\leq 5\cdot 10^4$) denoting the number of rounds.</p><p>Each of the next $t$ lines contain a single string $s$ ($1\leq |s|\leq 2\cdot 10^5$) consisting of lowercase English letters, denoting the string used for the round. Here $|s|$ denotes the length of the string $s$.</p><p>It is guaranteed that the sum of $|s|$ over all rounds does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each round, print a single line containing a string and an integer. If Alice wins the round, the string must be "<span class="tex-font-style-tt">Alice</span>". If Bob wins the round, the string must be "<span class="tex-font-style-tt">Bob</span>". The integer must be the difference between their scores assuming both players play optimally.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1\leq t\leq 5\cdot 10^4$) denoting the number of rounds.</p><p>Each of the next $t$ lines contain a single string $s$ ($1\leq |s|\leq 2\cdot 10^5$) consisting of lowercase English letters, denoting the string used for the round. Here $|s|$ denotes the length of the string $s$.</p><p>It is guaranteed that the sum of $|s|$ over all rounds does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each round, print a single line containing a string and an integer. If Alice wins the round, the string must be "<span class="tex-font-style-tt">Alice</span>". If Bob wins the round, the string must be "<span class="tex-font-style-tt">Bob</span>". The integer must be the difference between their scores assuming both players play optimally.</p>





```input1
5
aba
abc
cba
n
codeforces
```




```output1
Alice 2
Alice 4
Alice 4
Bob 14
Alice 93
```



## Note

<p>For the first round, $\texttt{"aba"}\xrightarrow{\texttt{Alice}}\texttt{"}{\color{red}{\texttt{ab}}}\texttt{a"}\xrightarrow{} \texttt{"a"}\xrightarrow{\texttt{Bob}}\texttt{"}{\color{red}{\texttt{a}}}\texttt{"}\xrightarrow{}\texttt{""}$. Alice's total score is $1+2=3$. Bob's total score is $1$.</p><p>For the second round, $\texttt{"abc"}\xrightarrow{\texttt{Alice}}\texttt{"a}{\color{red}{\texttt{bc}}}\texttt{"}\xrightarrow{} \texttt{"a"}\xrightarrow{\texttt{Bob}}\texttt{"}{\color{red}{\texttt{a}}}\texttt{"}\xrightarrow{}\texttt{""}$. Alice's total score is $2+3=5$. Bob's total score is $1$.</p><p>For the third round, $\texttt{"cba"}\xrightarrow{\texttt{Alice}}\texttt{"}{\color{red}{\texttt{cb}}}\texttt{a"}\xrightarrow{} \texttt{"a"}\xrightarrow{\texttt{Bob}}\texttt{"}{\color{red}{\texttt{a}}}\texttt{"}\xrightarrow{}\texttt{""}$. Alice's total score is $3+2=5$. Bob's total score is $1$.</p><p>For the fourth round, $\texttt{"n"}\xrightarrow{\texttt{Alice}}\texttt{"n"}\xrightarrow{} \texttt{"n"}\xrightarrow{\texttt{Bob}}\texttt{"}{\color{red}{\texttt{n}}}\texttt{"}\xrightarrow{}\texttt{""}$. Alice's total score is $0$. Bob's total score is $14$.</p><p>For the fifth round, $\texttt{"codeforces"}\xrightarrow{\texttt{Alice}}\texttt{"}{\color{red}{\texttt{codeforces}}}\texttt{"}\xrightarrow{} \texttt{""}$. Alice's total score is $3+15+4+5+6+15+18+3+5+19=93$. Bob's total score is $0$.</p>
