## Description

<div><p>There are $n$ football teams in the world. </p><p>The Main Football Organization (MFO) wants to host at most $m$ games. MFO wants the $i$-th game to be played between the teams $a_i$ and $b_i$ in one of the $k$ stadiums. </p><p>Let $s_{ij}$ be the numbers of games the $i$-th team played in the $j$-th stadium. MFO does not want a team to have much more games in one stadium than in the others. Therefore, for each team $i$, the absolute difference between the maximum and minimum among $s_{i1}, s_{i2}, \ldots, s_{ik}$ should not exceed $2$.</p><p>Each team has $w_i$&nbsp;— the amount of money MFO will earn for <span class="tex-font-style-bf">each</span> game of the $i$-th team. If the $i$-th team plays $l$ games, MFO will earn $w_i \cdot l$.</p><p>MFO needs to find what games in what stadiums they need to host in order to earn as much money as possible, not violating the rule they set.</p><p>However, this problem is too complicated for MFO. Therefore, they are asking you to help them.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, $k$ ($3 \leq n \leq 100$, $0 \leq m \leq 1\,000$, $1 \leq k \leq 1\,000$)&nbsp;— the number of teams, the number of games, and the number of stadiums.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($1 \leq w_i \leq 1\,000$)&nbsp;— the amount of money MFO will earn for each game of the $i$-th game.</p><p>Each of the following $m$ lines contains two integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$)&nbsp;— the teams that can play the $i$-th game. It is guaranteed that each pair of teams can play at most one game.</p></div><div class="output-specification"><p>For each game in the same order, print $t_i$ ($1 \leq t_i \leq k$)&nbsp;— the number of the stadium, in which $a_i$ and $b_i$ will play the game. If the $i$-th game should not be played, $t_i$ should be equal to $0$.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, $k$ ($3 \leq n \leq 100$, $0 \leq m \leq 1\,000$, $1 \leq k \leq 1\,000$)&nbsp;— the number of teams, the number of games, and the number of stadiums.</p><p>The second line contains $n$ integers $w_1, w_2, \ldots, w_n$ ($1 \leq w_i \leq 1\,000$)&nbsp;— the amount of money MFO will earn for each game of the $i$-th game.</p><p>Each of the following $m$ lines contains two integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$, $a_i \neq b_i$)&nbsp;— the teams that can play the $i$-th game. It is guaranteed that each pair of teams can play at most one game.</p>

## Output

<p>For each game in the same order, print $t_i$ ($1 \leq t_i \leq k$)&nbsp;— the number of the stadium, in which $a_i$ and $b_i$ will play the game. If the $i$-th game should not be played, $t_i$ should be equal to $0$.</p><p>If there are multiple answers, print any.</p>





```input1
7 11 3
4 7 8 10 10 9 3
6 2
6 1
7 6
4 3
4 6
3 1
5 3
7 5
7 3
4 2
1 4
```




```output1
3
2
1
1
3
1
2
1
2
3
2
```



## Note

<p>One of possible solutions to the example is shown below:</p><center> <img class="tex-graphics" src="file://tVk6VKKb.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
