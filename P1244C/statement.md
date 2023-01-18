## Description

<div><p>The football season has just ended in Berland. According to the rules of Berland football, each match is played between two teams. The result of each match is either a draw, or a victory of one of the playing teams. If a team wins the match, it gets $w$ points, and the opposing team gets $0$ points. If the game results in a draw, both teams get $d$ points.</p><p>The manager of the Berland capital team wants to summarize the results of the season, but, unfortunately, all information about the results of each match is lost. The manager only knows that the team has played $n$ games and got $p$ points for them.</p><p>You have to determine three integers $x$, $y$ and $z$ — the number of wins, draws and loses of the team. If there are multiple answers, print any of them. If there is no suitable triple $(x, y, z)$, report about it.</p></div><div class="input-specification"><p>The first line contains four integers $n$, $p$, $w$ and $d$ $(1 \le n \le 10^{12}, 0 \le p \le 10^{17}, 1 \le d &lt; w \le 10^{5})$ — the number of games, the number of points the team got, the number of points awarded for winning a match, and the number of points awarded for a draw, respectively. Note that $w &gt; d$, so the number of points awarded for winning is strictly greater than the number of points awarded for draw.</p></div><div class="output-specification"><p>If there is no answer, print $-1$.</p><p>Otherwise print three non-negative integers $x$, $y$ and $z$ — the number of wins, draws and losses of the team. If there are multiple possible triples $(x, y, z)$, print any of them. The numbers should meet the following conditions: </p><ul> <li> $x \cdot w + y \cdot d = p$, </li><li> $x + y + z = n$. </li></ul></div>

## Input

<p>The first line contains four integers $n$, $p$, $w$ and $d$ $(1 \le n \le 10^{12}, 0 \le p \le 10^{17}, 1 \le d &lt; w \le 10^{5})$ — the number of games, the number of points the team got, the number of points awarded for winning a match, and the number of points awarded for a draw, respectively. Note that $w &gt; d$, so the number of points awarded for winning is strictly greater than the number of points awarded for draw.</p>

## Output

<p>If there is no answer, print $-1$.</p><p>Otherwise print three non-negative integers $x$, $y$ and $z$ — the number of wins, draws and losses of the team. If there are multiple possible triples $(x, y, z)$, print any of them. The numbers should meet the following conditions: </p><ul> <li> $x \cdot w + y \cdot d = p$, </li><li> $x + y + z = n$. </li></ul>





```input1
30 60 3 1
```




```input2
10 51 5 4
```




```input3
20 0 15 5
```




```output1
17 9 4
```




```output2
-1
```




```output3
0 0 20
```



## Note

<p>One of the possible answers in the first example — $17$ wins, $9$ draws and $4$ losses. Then the team got $17 \cdot 3 + 9 \cdot 1 = 60$ points in $17 + 9 + 4 = 30$ games.</p><p>In the second example the maximum possible score is $10 \cdot 5 = 50$. Since $p = 51$, there is no answer.</p><p>In the third example the team got $0$ points, so all $20$ games were lost.</p>
