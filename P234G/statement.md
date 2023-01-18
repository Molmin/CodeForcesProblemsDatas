## Description

<div><p>Little time is left before Berland annual football championship. Therefore the coach of team "Losewille Rangers" decided to resume the practice, that were indefinitely interrupted for uncertain reasons. Overall there are <span class="tex-span"><i>n</i></span> players in "Losewille Rangers". Each player on the team has a number — a unique integer from 1 to <span class="tex-span"><i>n</i></span>. To prepare for the championship, the coach Mr. Floppe decided to spend some number of practices.</p><p>Mr. Floppe spent some long nights of his holiday planning how to conduct the practices. He came to a very complex practice system. Each practice consists of one game, all <span class="tex-span"><i>n</i></span> players of the team take part in the game. The players are sorted into two teams in some way. In this case, the teams may have different numbers of players, but each team must have at least one player.</p><p>The coach wants to be sure that after the series of the practice sessions each pair of players had at least one practice, when they played in different teams. As the players' energy is limited, the coach wants to achieve the goal in the least number of practices.</p><p>Help him to schedule the practices.</p></div><div class="input-specification"><p>A single input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>m</i></span> — the minimum number of practices the coach will have to schedule. Then print the descriptions of the practices in <span class="tex-span"><i>m</i></span> lines.</p><p>In the <span class="tex-span"><i>i</i></span>-th of those lines print <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> — the number of players in the first team during the <span class="tex-span"><i>i</i></span>-th practice (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the numbers of players in the first team. The rest of the players will play in the second team during this practice. Separate numbers on a line with spaces. Print the numbers of the players in any order. If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>A single input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>).</p>

## Output

<p>In the first line print <span class="tex-span"><i>m</i></span> — the minimum number of practices the coach will have to schedule. Then print the descriptions of the practices in <span class="tex-span"><i>m</i></span> lines.</p><p>In the <span class="tex-span"><i>i</i></span>-th of those lines print <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> — the number of players in the first team during the <span class="tex-span"><i>i</i></span>-th practice (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the numbers of players in the first team. The rest of the players will play in the second team during this practice. Separate numbers on a line with spaces. Print the numbers of the players in any order. If there are multiple optimal solutions, print any of them.</p>





```input1
2

```




```input2
3

```




```output1
1
1 1

```




```output2
2
2 1 2
1 1

```


