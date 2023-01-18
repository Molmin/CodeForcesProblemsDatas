## Description

<div><p><span class="tex-font-style-it">Any resemblance to any real championship and sport is accidental.</span></p><p>The Berland National team takes part in the local Football championship which now has a group stage. Let's describe the formal rules of the local championship: </p><ul> <li> the team that kicked most balls in the enemy's goal area wins the game; </li><li> the victory gives 3 point to the team, the draw gives 1 point and the defeat gives 0 points; </li><li> a group consists of four teams, the teams are ranked by the results of six games: each team plays exactly once with each other team; </li><li> the teams that get places 1 and 2 in the group stage results, go to the next stage of the championship. </li></ul><p>In the group stage the team's place is defined by the total number of scored points: the more points, the higher the place is. If two or more teams have the same number of points, then the following criteria are used (the criteria are listed in the order of falling priority, starting from the most important one): </p><ul> <li> the difference between the total number of scored goals and the total number of missed goals in the championship: the team with a higher value gets a higher place; </li><li> the total number of scored goals in the championship: the team with a higher value gets a higher place; </li><li> the lexicographical order of the name of the teams' countries: the country with the lexicographically smaller name gets a higher place. </li></ul><p>The Berland team plays in the group where the results of 5 out of 6 games are already known. To be exact, there is the last game left. There the Berand national team plays with some other team. The coach asks you to find such score <span class="tex-font-style-tt"><span class="tex-span"><i>X</i></span>:<span class="tex-span"><i>Y</i></span></span> (where <span class="tex-span"><i>X</i></span> is the number of goals Berland scored and <span class="tex-span"><i>Y</i></span> is the number of goals the opponent scored in the game), that fulfills the following conditions: </p><ul> <li> <span class="tex-span"><i>X</i></span> &gt; <span class="tex-span"><i>Y</i></span>, that is, Berland is going to win this game; </li><li> after the game Berland gets the 1st or the 2nd place in the group; </li><li> if there are multiple variants, you should choose such score <span class="tex-font-style-tt"><span class="tex-span"><i>X</i></span>:<span class="tex-span"><i>Y</i></span></span>, where value <span class="tex-span"><i>X</i> - <i>Y</i></span> is minimum; </li><li> if it is still impossible to come up with one score, you should choose the score where value <span class="tex-span"><i>Y</i></span> (the number of goals Berland misses) is minimum. </li></ul></div><div class="input-specification"><p>The input has five lines.</p><p>Each line describes a game as "<span class="tex-font-style-tt"><span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>goals</i><sub class="lower-index">1</sub></span>:<span class="tex-span"><i>goals</i><sub class="lower-index">2</sub></span></span>" (without the quotes), what means that team <span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> played a game with team <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span>, besides, <span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> scored <span class="tex-span"><i>goals</i><sub class="lower-index">1</sub></span> goals and <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span> scored <span class="tex-span"><i>goals</i><sub class="lower-index">2</sub></span> goals. The names of teams <span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span> are non-empty strings, consisting of uppercase English letters, with length of no more than 20 characters; <span class="tex-span"><i>goals</i><sub class="lower-index">1</sub>, <i>goals</i><sub class="lower-index">2</sub></span> are integers from 0 to 9. </p><p>The Berland team is called "BERLAND". It is guaranteed that the Berland team and one more team played exactly 2 games and the the other teams played exactly 3 games.</p></div><div class="output-specification"><p>Print the required score in the last game as <span class="tex-font-style-tt"><span class="tex-span"><i>X</i></span>:<span class="tex-span"><i>Y</i></span></span>, where <span class="tex-span"><i>X</i></span> is the number of goals Berland scored and <span class="tex-span"><i>Y</i></span> is the number of goals the opponent scored. If the Berland team does not get the first or the second place in the group, whatever this game's score is, then print on a single line "IMPOSSIBLE" (without the quotes).</p><p>Note, that the result score can be very huge, 10:0 for example.</p></div>

## Input

<p>The input has five lines.</p><p>Each line describes a game as "<span class="tex-font-style-tt"><span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>goals</i><sub class="lower-index">1</sub></span>:<span class="tex-span"><i>goals</i><sub class="lower-index">2</sub></span></span>" (without the quotes), what means that team <span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> played a game with team <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span>, besides, <span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> scored <span class="tex-span"><i>goals</i><sub class="lower-index">1</sub></span> goals and <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span> scored <span class="tex-span"><i>goals</i><sub class="lower-index">2</sub></span> goals. The names of teams <span class="tex-span"><i>team</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>team</i><sub class="lower-index">2</sub></span> are non-empty strings, consisting of uppercase English letters, with length of no more than 20 characters; <span class="tex-span"><i>goals</i><sub class="lower-index">1</sub>, <i>goals</i><sub class="lower-index">2</sub></span> are integers from 0 to 9. </p><p>The Berland team is called "BERLAND". It is guaranteed that the Berland team and one more team played exactly 2 games and the the other teams played exactly 3 games.</p>

## Output

<p>Print the required score in the last game as <span class="tex-font-style-tt"><span class="tex-span"><i>X</i></span>:<span class="tex-span"><i>Y</i></span></span>, where <span class="tex-span"><i>X</i></span> is the number of goals Berland scored and <span class="tex-span"><i>Y</i></span> is the number of goals the opponent scored. If the Berland team does not get the first or the second place in the group, whatever this game's score is, then print on a single line "IMPOSSIBLE" (without the quotes).</p><p>Note, that the result score can be very huge, 10:0 for example.</p>





```input1
AERLAND DERLAND 2:1
DERLAND CERLAND 0:3
CERLAND AERLAND 0:1
AERLAND BERLAND 2:0
DERLAND BERLAND 4:0

```




```input2
AERLAND DERLAND 2:2
DERLAND CERLAND 2:3
CERLAND AERLAND 1:3
AERLAND BERLAND 2:1
DERLAND BERLAND 4:1

```




```output1
6:0

```




```output2
IMPOSSIBLE

```



## Note

<p>In the first sample "BERLAND" plays the last game with team "CERLAND". If Berland wins with score 6:0, the results' table looks like that in the end: </p><ol> <li> AERLAND (points: 9, the difference between scored and missed goals: 4, scored goals: 5) </li><li> BERLAND (points: 3, the difference between scored and missed goals: 0, scored goals: 6) </li><li> DERLAND (points: 3, the difference between scored and missed goals: 0, scored goals: 5) </li><li> CERLAND (points: 3, the difference between scored and missed goals: -4, scored goals: 3) </li></ol><p>In the second sample teams "AERLAND" and "DERLAND" have already won 7 and 4 points, respectively. The Berland team wins only 3 points, which is not enough to advance to the next championship stage.</p>
