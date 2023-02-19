## Description

<div><p>$2^n$ teams participate in a playoff tournament. The tournament consists of $2^n - 1$ games. They are held as follows: in the first phase of the tournament, the teams are split into pairs: team $1$ plays against team $2$, team $3$ plays against team $4$, and so on (so, $2^{n-1}$ games are played in that phase). When a team loses a game, it is eliminated, and each game results in elimination of one team (there are no ties). After that, only $2^{n-1}$ teams remain. If only one team remains, it is declared the champion; otherwise, the second phase begins, where $2^{n-2}$ games are played: in the first one of them, the winner of the game "$1$ vs $2$" plays against the winner of the game "$3$ vs $4$", then the winner of the game "$5$ vs $6$" plays against the winner of the game "$7$ vs $8$", and so on. This process repeats until only one team remains. </p><p>The skill level of the $i$-th team is $p_i$, where $p$ is a permutation of integers $1$, $2$, ..., $2^n$ (a permutation is an array where each element from $1$ to $2^n$ occurs exactly once).</p><p>You are given a string $s$ which consists of $n$ characters. These characters denote the results of games in each phase of the tournament as follows: </p><ul> <li> if $s_i$ is equal to <span class="tex-font-style-tt">0</span>, then during the $i$-th phase (the phase with $2^{n-i}$ games), in each match, the team with the lower skill level wins; </li><li> if $s_i$ is equal to <span class="tex-font-style-tt">1</span>, then during the $i$-th phase (the phase with $2^{n-i}$ games), in each match, the team with the higher skill level wins. </li></ul><p>Let's say that an integer $x$ is <span class="tex-font-style-bf">winning</span> if it is possible to find a permutation $p$ such that the team with skill $x$ wins the tournament. Find all winning integers.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 18$).</p><p>The second line contains the string $s$ of length $n$ consisting of the characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>Print all the winning integers $x$ in ascending order.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 18$).</p><p>The second line contains the string $s$ of length $n$ consisting of the characters <span class="tex-font-style-tt">0</span> and/or <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>Print all the winning integers $x$ in ascending order.</p>





```input1
3
101
```




```input2
1
1
```




```input3
2
01
```




```output1
4 5 6 7
```




```output2
2
```




```output3
2 3
```


