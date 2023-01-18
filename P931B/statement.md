## Description

<div><p>The last stage of Football World Cup is played using the play-off system.</p><p>There are <span class="tex-span"><i>n</i></span> teams left in this stage, they are enumerated from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Several rounds are held, in each round the remaining teams are sorted in the order of their ids, then the first in this order plays with the second, the third&nbsp;— with the fourth, the fifth&nbsp;— with the sixth, and so on. It is guaranteed that in each round there is even number of teams. The winner of each game advances to the next round, the loser is eliminated from the tournament, there are no draws. In the last round there is the only game with two remaining teams: the round is called the Final, the winner is called the champion, and the tournament is over.</p><p>Arkady wants his two favorite teams to play in the Final. Unfortunately, the team ids are already determined, and it may happen that it is impossible for teams to meet in the Final, because they are to meet in some earlier stage, if they are strong enough. Determine, in which round the teams with ids <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> can meet.</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 256</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the total number of teams, and the ids of the teams that Arkady is interested in. </p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is such that in each round an even number of team advance, and that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are not equal.</p></div><div class="output-specification"><p>In the only line print "<span class="tex-font-style-tt">Final!</span>" (without quotes), if teams <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> can meet in the Final.</p><p>Otherwise, print a single integer&nbsp;— the number of the round in which teams <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> can meet. The round are enumerated from <span class="tex-span">1</span>.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 256</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the total number of teams, and the ids of the teams that Arkady is interested in. </p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is such that in each round an even number of team advance, and that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are not equal.</p>

## Output

<p>In the only line print "<span class="tex-font-style-tt">Final!</span>" (without quotes), if teams <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> can meet in the Final.</p><p>Otherwise, print a single integer&nbsp;— the number of the round in which teams <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> can meet. The round are enumerated from <span class="tex-span">1</span>.</p>





```input1
4 1 2

```




```input2
8 2 6

```




```input3
8 7 5

```




```output1
1

```




```output2
Final!

```




```output3
2

```



## Note

<p>In the first example teams <span class="tex-span">1</span> and <span class="tex-span">2</span> meet in the first round.</p><p>In the second example teams <span class="tex-span">2</span> and <span class="tex-span">6</span> can only meet in the third round, which is the Final, if they win all their opponents in earlier rounds.</p><p>In the third example the teams with ids <span class="tex-span">7</span> and <span class="tex-span">5</span> can meet in the second round, if they win their opponents in the first round.</p>
