## Description

<div><p>$2^k$ teams participate in a playoff tournament. The tournament consists of $2^k - 1$ games. They are held as follows: first of all, the teams are split into pairs: team $1$ plays against team $2$, team $3$ plays against team $4$ (exactly in this order), and so on (so, $2^{k-1}$ games are played in that phase). When a team loses a game, it is eliminated, and each game results in elimination of one team (there are no ties). After that, only $2^{k-1}$ teams remain. If only one team remains, it is declared the champion; otherwise, $2^{k-2}$ games are played: in the first one of them, the winner of the game "$1$ vs $2$" plays against the winner of the game "$3$ vs $4$", then the winner of the game "$5$ vs $6$" plays against the winner of the game "$7$ vs $8$", and so on. This process repeats until only one team remains.</p><p>For example, this picture describes the chronological order of games with $k = 3$:</p><center> <img class="tex-graphics" src="file://TnJZti4y.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Let the string $s$ consisting of $2^k - 1$ characters describe the results of the games in chronological order as follows:</p><ul> <li> if $s_i$ is <span class="tex-font-style-tt">0</span>, then the team with lower index wins the $i$-th game; </li><li> if $s_i$ is <span class="tex-font-style-tt">1</span>, then the team with greater index wins the $i$-th game; </li><li> if $s_i$ is <span class="tex-font-style-tt">?</span>, then the result of the $i$-th game is unknown (any team could win this game). </li></ul><p>Let $f(s)$ be the number of <span class="tex-font-style-it">possible winners</span> of the tournament described by the string $s$. A team $i$ is a <span class="tex-font-style-it">possible winner</span> of the tournament if it is possible to replace every <span class="tex-font-style-tt">?</span> with either <span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">0</span> in such a way that team $i$ is the champion.</p><p>You are given the initial state of the string $s$. You have to process $q$ queries of the following form: </p><ul> <li> $p$ $c$&nbsp;— replace $s_p$ with character $c$, and print $f(s)$ as the result of the query. </li></ul></div><div class="input-specification"><p>The first line contains one integer $k$ ($1 \le k \le 18$).</p><p>The second line contains a string consisting of $2^k - 1$ characters&nbsp;— the initial state of the string $s$. Each character is either <span class="tex-font-style-tt">?</span>, <span class="tex-font-style-tt">0</span>, or <span class="tex-font-style-tt">1</span>.</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Then $q$ lines follow, the $i$-th line contains an integer $p$ and a character $c$ ($1 \le p \le 2^k - 1$; $c$ is either <span class="tex-font-style-tt">?</span>, <span class="tex-font-style-tt">0</span>, or <span class="tex-font-style-tt">1</span>), describing the $i$-th query.</p></div><div class="output-specification"><p>For each query, print one integer&nbsp;— $f(s)$.</p></div>

## Input

<p>The first line contains one integer $k$ ($1 \le k \le 18$).</p><p>The second line contains a string consisting of $2^k - 1$ characters&nbsp;— the initial state of the string $s$. Each character is either <span class="tex-font-style-tt">?</span>, <span class="tex-font-style-tt">0</span>, or <span class="tex-font-style-tt">1</span>.</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;— the number of queries.</p><p>Then $q$ lines follow, the $i$-th line contains an integer $p$ and a character $c$ ($1 \le p \le 2^k - 1$; $c$ is either <span class="tex-font-style-tt">?</span>, <span class="tex-font-style-tt">0</span>, or <span class="tex-font-style-tt">1</span>), describing the $i$-th query.</p>

## Output

<p>For each query, print one integer&nbsp;— $f(s)$.</p>





```input1
3
0110?11
6
5 1
6 ?
7 ?
1 ?
5 ?
1 1
```




```output1
1
2
3
3
5
4
```


