## Description

<div><p>Iron and Werewolf are participating in a chess Olympiad, so they want to practice team building. They gathered $n$ players, where $n$ is a power of $2$, and they will play sports. Iron and Werewolf are among those $n$ people.</p><p>One of the sports is tug of war. For each $1\leq i \leq n$, the $i$-th player has <span class="tex-font-style-it">strength</span> $s_i$. Elimination rounds will be held until only one player remains&nbsp;— we call that player the <span class="tex-font-style-it">absolute winner</span>.</p><p>In each round: </p><ul> <li> Assume that $m&gt;1$ players are still in the game, where $m$ is a power of $2$. </li><li> The $m$ players are split into two teams of equal sizes (i.&nbsp;e., with $m/2$ players in each team). The strength of a team is the sum of the strengths of its players. </li><li> If the teams have equal strengths, Iron chooses who wins; otherwise, the stronger team wins. </li><li> Every player in the losing team is eliminated, so $m/2$ players remain. </li></ul><p>Iron already knows each player's strength and is wondering who can become the absolute winner and who can't if he may choose how the teams will be formed in each round, as well as the winning team in case of equal <span class="tex-font-style-it">strengths</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($4 \leq n \leq 32$)&nbsp;— the number of players participating in tug of war. It is guaranteed that $n$ is a power of $2$.</p><p>The second line consists of a sequence $s_1,s_2, \ldots, s_n$ of integers ($1 \leq s_i \leq 10^{15}$)&nbsp;— the strengths of the players.</p></div><div class="output-specification"><p>In a single line output a binary string $s$ of length $n$&nbsp;— the $i$-th character of $s$ should be $1$ if the $i$-th player can become the <span class="tex-font-style-it">absolute winner</span> and it should be $0$ otherwise.</p></div>

## Input

<p>The first line contains a single integer $n$ ($4 \leq n \leq 32$)&nbsp;— the number of players participating in tug of war. It is guaranteed that $n$ is a power of $2$.</p><p>The second line consists of a sequence $s_1,s_2, \ldots, s_n$ of integers ($1 \leq s_i \leq 10^{15}$)&nbsp;— the strengths of the players.</p>

## Output

<p>In a single line output a binary string $s$ of length $n$&nbsp;— the $i$-th character of $s$ should be $1$ if the $i$-th player can become the <span class="tex-font-style-it">absolute winner</span> and it should be $0$ otherwise.</p>





```input1
4
60 32 59 87
```




```input2
4
100 100 100 100
```




```input3
8
8 8 8 8 4 4 4 4
```




```input4
32
1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32
```




```input5
16
1 92875987325987 1 1 92875987325986 92875987325985 1 92875987325988 92875987325990 92875987325989 1 1 92875987325984 92875987325983 1 1
```




```output1
1001
```




```output2
1111
```




```output3
11110000
```




```output4
00000000000000001111111111111111
```




```output5
0100110111001000
```



## Note

<p>In the first example, players $1$ and $4$ with their respective strengths of $60$ and $87$ can become the <span class="tex-font-style-it">absolute winners</span>.</p><p>Let's describe the process for player $1$. Firstly, we divide the players into teams $[1,3]$ and $[2,4]$. <span class="tex-font-style-it">Strengths</span> of those two teams are $60+59=119$ and $32+87=119$. They they are equal, Iron can choose to disqualify any of the two teams. Let his choice be the second team.</p><p>We are left with players $1$ and $3$. Since $1$ has greater strength ($60&gt;59$) they win and are declared the <span class="tex-font-style-it">absolute winner</span> as they are the last remaining player.</p><p>In the third example, the strengths of the remaining players may look like $[8,8,8,8,4,4,4,4] \rightarrow [8,8,4,4] \rightarrow [8,4] \rightarrow [8]$. Each person with strength $8$ can become the <span class="tex-font-style-it">absolute winner</span> and it can be proved that others can't.</p>
