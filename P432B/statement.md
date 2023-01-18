## Description

<div><p>Consider a football tournament where <span class="tex-span"><i>n</i></span> teams participate. Each team has two football kits: for home games, and for away games. The kit for home games of the <span class="tex-span"><i>i</i></span>-th team has color <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and the kit for away games of this team has color <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>In the tournament, each team plays exactly one home game and exactly one away game with each other team (<span class="tex-span"><i>n</i>(<i>n</i> - 1)</span> games in total). The team, that plays the home game, traditionally plays in its home kit. The team that plays an away game plays in its away kit. However, if two teams has the kits of the same color, they cannot be distinguished. In this case the away team plays in its home kit.</p><p>Calculate how many games in the described tournament each team plays in its home kit and how many games it plays in its away kit.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of teams. Next <span class="tex-span"><i>n</i></span> lines contain the description of the teams. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> — the color numbers for the home and away kits of the <span class="tex-span"><i>i</i></span>-th team.</p></div><div class="output-specification"><p>For each team, print on a single line two space-separated integers — the number of games this team is going to play in home and away kits, correspondingly. Print the answers for the teams in the order they appeared in the input.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of teams. Next <span class="tex-span"><i>n</i></span> lines contain the description of the teams. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> — the color numbers for the home and away kits of the <span class="tex-span"><i>i</i></span>-th team.</p>

## Output

<p>For each team, print on a single line two space-separated integers — the number of games this team is going to play in home and away kits, correspondingly. Print the answers for the teams in the order they appeared in the input.</p>





```input1
2
1 2
2 1

```




```input2
3
1 2
2 1
1 3

```




```output1
2 0
2 0

```




```output2
3 1
4 0
2 2

```


