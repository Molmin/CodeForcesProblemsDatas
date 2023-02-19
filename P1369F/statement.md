## Description

<div><p><span class="tex-font-style-it">Lee is used to finish his stories in a stylish way, this time he barely failed it, but Ice Bear came and helped him. Lee is so grateful for it, so he decided to show Ice Bear his new game called "Critic"...</span></p><p>The game is a one versus one game. It has $t$ rounds, each round has two integers $s_i$ and $e_i$ (which are determined and are known before the game begins, $s_i$ and $e_i$ may differ from round to round). The integer $s_i$ is written on the board at the beginning of the corresponding round. </p><p>The players will take turns. Each player will erase the number on the board (let's say it was $a$) and will choose to write either $2 \cdot a$ or $a + 1$ instead. Whoever writes a number strictly greater than $e_i$ loses that round and the other one wins that round.</p><p>Now Lee wants to play "Critic" against Ice Bear, for each round he has chosen the round's $s_i$ and $e_i$ in advance. Lee will start the first round, the loser of each round will start the next round.</p><p>The winner of the last round is the winner of the game, and the loser of the last round is the loser of the game.</p><p>Determine if Lee can be the winner independent of Ice Bear's moves or not. Also, determine if Lee can be the loser independent of Ice Bear's moves or not.</p></div><div class="input-specification"><p>The first line contains the integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of rounds the game has. </p><p>Then $t$ lines follow, each contains two integers $s_i$ and $e_i$ ($1 \le s_i \le e_i \le 10^{18}$)&nbsp;— the $i$-th round's information.</p><p>The rounds are played in the same order as given in input, $s_i$ and $e_i$ for all rounds are known to everyone before the game starts.</p></div><div class="output-specification"><p>Print two integers.</p><p>The first one should be <span class="tex-font-style-tt">1</span> if Lee can be the winner independent of Ice Bear's moves, and <span class="tex-font-style-tt">0</span> otherwise.</p><p>The second one should be <span class="tex-font-style-tt">1</span> if Lee can be the loser independent of Ice Bear's moves, and <span class="tex-font-style-tt">0</span> otherwise.</p></div>

## Input

<p>The first line contains the integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of rounds the game has. </p><p>Then $t$ lines follow, each contains two integers $s_i$ and $e_i$ ($1 \le s_i \le e_i \le 10^{18}$)&nbsp;— the $i$-th round's information.</p><p>The rounds are played in the same order as given in input, $s_i$ and $e_i$ for all rounds are known to everyone before the game starts.</p>

## Output

<p>Print two integers.</p><p>The first one should be <span class="tex-font-style-tt">1</span> if Lee can be the winner independent of Ice Bear's moves, and <span class="tex-font-style-tt">0</span> otherwise.</p><p>The second one should be <span class="tex-font-style-tt">1</span> if Lee can be the loser independent of Ice Bear's moves, and <span class="tex-font-style-tt">0</span> otherwise.</p>





```input1
3
5 8
1 4
3 10
```




```input2
4
1 2
2 3
3 4
4 5
```




```input3
1
1 1
```




```input4
2
1 9
4 5
```




```input5
2
1 2
2 8
```




```input6
6
216986951114298167 235031205335543871
148302405431848579 455670351549314242
506251128322958430 575521452907339082
1 768614336404564650
189336074809158272 622104412002885672
588320087414024192 662540324268197150
```




```output1
1 1
```




```output2
0 0
```




```output3
0 1
```




```output4
0 0
```




```output5
1 0
```




```output6
1 0
```



## Note

<p>Remember, whoever writes an integer greater than $e_i$ loses.</p>
