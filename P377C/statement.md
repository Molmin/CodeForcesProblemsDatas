## Description

<div><p>Kostya is a progamer specializing in the discipline of Dota 2. Valve Corporation, the developer of this game, has recently released a new patch which turned the balance of the game upside down. Kostya, as the captain of the team, realizes that the greatest responsibility lies on him, so he wants to resort to the analysis of innovations patch from the mathematical point of view to choose the best heroes for his team in every game.</p><p>A Dota 2 match involves two teams, each of them must choose some heroes that the players of the team are going to play for, and it is forbidden to choose the same hero several times, even in different teams. In large electronic sports competitions where Kostya's team is going to participate, the matches are held in the Captains Mode. In this mode the captains select the heroes by making one of two possible actions in a certain, predetermined order: pick or ban.</p><ul> <li> To pick a hero for the team. After the captain picks, the picked hero goes to his team (later one of a team members will play it) and can no longer be selected by any of the teams. </li><li> To ban a hero. After the ban the hero is not sent to any of the teams, but it still can no longer be selected by any of the teams. </li></ul><p>The team captain may miss a pick or a ban. If he misses a pick, a random hero is added to his team from those that were available at that moment, and if he misses a ban, no hero is banned, as if there was no ban.</p><p>Kostya has already identified the strength of all the heroes based on the new patch fixes. Of course, Kostya knows the order of picks and bans. The strength of a team is the sum of the strengths of the team's heroes and both teams that participate in the match seek to maximize the difference in strengths in their favor. Help Kostya determine what team, the first one or the second one, has advantage in the match, and how large the advantage is.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of heroes in Dota 2.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the strengths of all the heroes.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>, 20)</span>)&nbsp;— the number of actions the captains of the team must perform.</p><p>Next <span class="tex-span"><i>m</i></span> lines look like "<span class="tex-span"><i>action</i>&nbsp;<i>team</i></span>", where <span class="tex-span"><i>action</i></span> is the needed action: a pick (represented as a "<span class="tex-font-style-tt">p</span>") or a ban (represented as a "<span class="tex-font-style-tt">b</span>"), and <span class="tex-span"><i>team</i></span> is the number of the team that needs to perform the action (number <span class="tex-span">1</span> or <span class="tex-span">2</span>).</p><p>It is guaranteed that each team makes at least one pick. Besides, each team has the same number of picks and the same number of bans.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the difference between the strength of the first team and the strength of the second team if the captains of both teams will act optimally well.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of heroes in Dota 2.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the strengths of all the heroes.</p><p>The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>, 20)</span>)&nbsp;— the number of actions the captains of the team must perform.</p><p>Next <span class="tex-span"><i>m</i></span> lines look like "<span class="tex-span"><i>action</i>&nbsp;<i>team</i></span>", where <span class="tex-span"><i>action</i></span> is the needed action: a pick (represented as a "<span class="tex-font-style-tt">p</span>") or a ban (represented as a "<span class="tex-font-style-tt">b</span>"), and <span class="tex-span"><i>team</i></span> is the number of the team that needs to perform the action (number <span class="tex-span">1</span> or <span class="tex-span">2</span>).</p><p>It is guaranteed that each team makes at least one pick. Besides, each team has the same number of picks and the same number of bans.</p>

## Output

<p>Print a single integer&nbsp;— the difference between the strength of the first team and the strength of the second team if the captains of both teams will act optimally well.</p>





```input1
2
2 1
2
p 1
p 2

```




```input2
6
6 4 5 4 5 5
4
b 2
p 1
b 1
p 2

```




```input3
4
1 2 3 4
4
p 2
b 2
p 1
b 1

```




```output1
1

```




```output2
0

```




```output3
-2

```


