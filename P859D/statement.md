## Description

<div><p>The annual college sports-ball tournament is approaching, which for trademark reasons we'll refer to as Third Month Insanity. There are a total of <span class="tex-span">2<sup class="upper-index"><i>N</i></sup></span> teams participating in the tournament, numbered from <span class="tex-span">1</span> to <span class="tex-span">2<sup class="upper-index"><i>N</i></sup></span>. The tournament lasts <span class="tex-span"><i>N</i></span> rounds, with each round eliminating half the teams. The first round consists of <span class="tex-span">2<sup class="upper-index"><i>N</i> - 1</sup></span> games, numbered starting from <span class="tex-span">1</span>. In game <span class="tex-span"><i>i</i></span>, team <span class="tex-span">2·<i>i</i> - 1</span> will play against team <span class="tex-span">2·<i>i</i></span>. The loser is eliminated and the winner advances to the next round (there are no ties). Each subsequent round has half as many games as the previous round, and in game <span class="tex-span"><i>i</i></span> the winner of the previous round's game <span class="tex-span">2·<i>i</i> - 1</span> will play against the winner of the previous round's game <span class="tex-span">2·<i>i</i></span>.</p><p>Every year the office has a pool to see who can create the best bracket. A bracket is a set of winner predictions for every game. For games in the first round you may predict either team to win, but for games in later rounds the winner you predict must also be predicted as a winner in the previous round. Note that the bracket is fully constructed before any games are actually played. Correct predictions in the first round are worth <span class="tex-span">1</span> point, and correct predictions in each subsequent round are worth twice as many points as the previous, so correct predictions in the final game are worth <span class="tex-span">2<sup class="upper-index"><i>N</i> - 1</sup></span> points.</p><p>For every pair of teams in the league, you have estimated the probability of each team winning if they play against each other. Now you want to construct a bracket with the maximum possible expected score.</p></div><div class="input-specification"><p>Input will begin with a line containing <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 6</span>).</p><p><span class="tex-span">2<sup class="upper-index"><i>N</i></sup></span> lines follow, each with <span class="tex-span">2<sup class="upper-index"><i>N</i></sup></span> integers. The <span class="tex-span"><i>j</i></span>-th column of the <span class="tex-span"><i>i</i></span>-th row indicates the percentage chance that team <span class="tex-span"><i>i</i></span> will defeat team <span class="tex-span"><i>j</i></span>, unless <span class="tex-span"><i>i</i> = <i>j</i></span>, in which case the value will be <span class="tex-span">0</span>. It is guaranteed that the <span class="tex-span"><i>i</i></span>-th column of the <span class="tex-span"><i>j</i></span>-th row plus the <span class="tex-span"><i>j</i></span>-th column of the <span class="tex-span"><i>i</i></span>-th row will add to exactly <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>Print the maximum possible expected score over all possible brackets. Your answer must be correct to within an absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer will be considered correct, if <img align="middle" class="tex-formula" src="file://E2bTnaEc.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>Input will begin with a line containing <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 6</span>).</p><p><span class="tex-span">2<sup class="upper-index"><i>N</i></sup></span> lines follow, each with <span class="tex-span">2<sup class="upper-index"><i>N</i></sup></span> integers. The <span class="tex-span"><i>j</i></span>-th column of the <span class="tex-span"><i>i</i></span>-th row indicates the percentage chance that team <span class="tex-span"><i>i</i></span> will defeat team <span class="tex-span"><i>j</i></span>, unless <span class="tex-span"><i>i</i> = <i>j</i></span>, in which case the value will be <span class="tex-span">0</span>. It is guaranteed that the <span class="tex-span"><i>i</i></span>-th column of the <span class="tex-span"><i>j</i></span>-th row plus the <span class="tex-span"><i>j</i></span>-th column of the <span class="tex-span"><i>i</i></span>-th row will add to exactly <span class="tex-span">100</span>.</p>

## Output

<p>Print the maximum possible expected score over all possible brackets. Your answer must be correct to within an absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer will be considered correct, if <img align="middle" class="tex-formula" src="file://E2bTnaEc.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2
0 40 100 100
60 0 40 40
0 60 0 45
0 60 55 0

```




```input2
3
0 0 100 0 100 0 0 0
100 0 100 0 0 0 100 100
0 0 0 100 100 0 0 0
100 100 0 0 0 0 100 100
0 100 0 100 0 0 100 0
100 100 100 100 100 0 0 0
100 0 100 0 0 100 0 0
100 0 100 0 100 100 100 0

```




```input3
2
0 21 41 26
79 0 97 33
59 3 0 91
74 67 9 0

```




```output1
1.75

```




```output2
12

```




```output3
3.141592

```



## Note

<p>In the first example, you should predict teams <span class="tex-span">1</span> and <span class="tex-span">4</span> to win in round <span class="tex-span">1</span>, and team <span class="tex-span">1</span> to win in round <span class="tex-span">2</span>. Recall that the winner you predict in round <span class="tex-span">2</span> must also be predicted as a winner in round <span class="tex-span">1</span>.</p>
