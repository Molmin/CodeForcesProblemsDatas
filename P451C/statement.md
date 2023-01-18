## Description

<div><p>There are <span class="tex-span"><i>n</i></span> games in a football tournament. Three teams are participating in it. Currently <span class="tex-span"><i>k</i></span> games had already been played. </p><p>You are an avid football fan, but recently you missed the whole <span class="tex-span"><i>k</i></span> games. Fortunately, you remember a guess of your friend for these <span class="tex-span"><i>k</i></span> games. Your friend did not tell exact number of wins of each team, instead he thought that absolute difference between number of wins of first and second team will be <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> and that of between second and third team will be <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span>.</p><p>You don't want any of team win the tournament, that is each team should have the same number of wins after <span class="tex-span"><i>n</i></span> games. That's why you want to know: does there exist a valid tournament satisfying the friend's guess such that no team will win this tournament?</p><p>Note that outcome of a match can not be a draw, it has to be either win or loss.</p></div><div class="input-specification"><p>The first line of the input contains a single integer corresponding to number of test cases <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines will contain four space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup>;&nbsp;0 ≤ <i>k</i> ≤ <i>n</i>;&nbsp;0 ≤ <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub> ≤ <i>k</i>)</span> — data for the current test case.</p></div><div class="output-specification"><p>For each test case, output a single line containing either "<span class="tex-font-style-tt">yes</span>" if it is possible to have no winner of tournament, or "<span class="tex-font-style-tt">no</span>" otherwise (without quotes).</p></div>

## Input

<p>The first line of the input contains a single integer corresponding to number of test cases <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines will contain four space-separated integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">12</sup>;&nbsp;0 ≤ <i>k</i> ≤ <i>n</i>;&nbsp;0 ≤ <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub> ≤ <i>k</i>)</span> — data for the current test case.</p>

## Output

<p>For each test case, output a single line containing either "<span class="tex-font-style-tt">yes</span>" if it is possible to have no winner of tournament, or "<span class="tex-font-style-tt">no</span>" otherwise (without quotes).</p>





```input1
5
3 0 0 0
3 3 0 0
6 4 1 0
6 3 3 0
3 3 3 2

```




```output1
yes
yes
yes
no
no

```



## Note

<p>Sample 1. There has not been any match up to now <span class="tex-span">(<i>k</i> = 0, <i>d</i><sub class="lower-index">1</sub> = 0, <i>d</i><sub class="lower-index">2</sub> = 0)</span>. If there will be three matches (1-2, 2-3, 3-1) and each team wins once, then at the end each team will have 1 win.</p><p>Sample 2. You missed all the games <span class="tex-span">(<i>k</i> = 3)</span>. As <span class="tex-span"><i>d</i><sub class="lower-index">1</sub> = 0</span> and <span class="tex-span"><i>d</i><sub class="lower-index">2</sub> = 0</span>, and there is a way to play three games with no winner of tournament (described in the previous sample), the answer is "<span class="tex-font-style-tt">yes</span>".</p><p>Sample 3. You missed 4 matches, and <span class="tex-span"><i>d</i><sub class="lower-index">1</sub> = 1, <i>d</i><sub class="lower-index">2</sub> = 0</span>. These four matches can be: 1-2 (win 2), 1-3 (win 3), 1-2 (win 1), 1-3 (win 1). Currently the first team has 2 wins, the second team has 1 win, the third team has 1 win. Two remaining matches can be: 1-2 (win 2), 1-3 (win 3). In the end all the teams have equal number of wins (2 wins).</p>
