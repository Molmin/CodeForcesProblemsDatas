## Description

<div><p>The biggest event of the year – Cota 2 world championship "The Innernational" is right around the corner. $2^n$ teams will compete in a double-elimination format (please, carefully read problem statement even if you know what is it) to identify the champion. </p><p>Teams are numbered from $1$ to $2^n$ and will play games one-on-one. All teams start in the upper bracket.</p><p>All upper bracket matches will be held played between teams that haven't lost any games yet. Teams are split into games by team numbers. Game winner advances in the next round of upper bracket, losers drop into the lower bracket.</p><p>Lower bracket starts with $2^{n-1}$ teams that lost the first upper bracket game. Each lower bracket round consists of two games. In the first game of a round $2^k$ teams play a game with each other (teams are split into games by team numbers). $2^{k-1}$ loosing teams are eliminated from the championship, $2^{k-1}$ winning teams are playing $2^{k-1}$ teams that got eliminated in this round of upper bracket (again, teams are split into games by team numbers). As a result of each round both upper and lower bracket have $2^{k-1}$ teams remaining. See example notes for better understanding.</p><p>Single remaining team of upper bracket plays with single remaining team of lower bracket in grand-finals to identify championship winner.</p><p>You are a fan of teams with numbers $a_1, a_2, ..., a_k$. You want the championship to have as many games with your favourite teams as possible. Luckily, you can affect results of every championship game the way you want. What's maximal possible number of championship games that include teams you're fan of?</p></div><div class="input-specification"><p>First input line has two integers $n, k$&nbsp;— $2^n$ teams are competing in the championship. You are a fan of $k$ teams ($2 \le n \le 17; 0 \le k \le 2^n$).</p><p>Second input line has $k$ distinct integers $a_1, \ldots, a_k$&nbsp;— numbers of teams you're a fan of ($1 \le a_i \le 2^n$).</p></div><div class="output-specification"><p>Output single integer&nbsp;— maximal possible number of championship games that include teams you're fan of.</p></div>

## Input

<p>First input line has two integers $n, k$&nbsp;— $2^n$ teams are competing in the championship. You are a fan of $k$ teams ($2 \le n \le 17; 0 \le k \le 2^n$).</p><p>Second input line has $k$ distinct integers $a_1, \ldots, a_k$&nbsp;— numbers of teams you're a fan of ($1 \le a_i \le 2^n$).</p>

## Output

<p>Output single integer&nbsp;— maximal possible number of championship games that include teams you're fan of.</p>





```input1
3 1
6
```




```input2
3 3
1 7 8
```




```input3
3 4
1 3 5 7
```




```output1
6
```




```output2
11
```




```output3
14
```



## Note

<p>On the image, each game of the championship is denoted with an English letter ($a$ to $n$). Winner of game $i$ is denoted as $Wi$, loser is denoted as $Li$. Teams you're a fan of are highlighted with red background.</p><p>In the first example, team $6$ will play in 6 games if it looses the first upper bracket game (game $c$) and wins all lower bracket games (games $h, j, l, m$). </p><center><img class="tex-graphics" src="file://rx5LCWCO.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In the second example, teams $7$ and $8$ have to play with each other in the first game of upper bracket (game $d$). Team $8$ can win all remaining games in upper bracket, when teams $1$ and $7$ will compete in the lower bracket. </p><center><img class="tex-graphics" src="file://zeEkf2xx.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In the third example, your favourite teams can play in all games of the championship. </p><center><img class="tex-graphics" src="file://vEPu6yn2.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
