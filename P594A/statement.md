## Description

<div><p><span class="tex-font-style-it">In the official contest this problem has a different statement, for which jury's solution was working incorrectly, and for this reason it was excluded from the contest. This mistake have been fixed and the current given problem statement and model solution corresponds to what jury wanted it to be during the contest.</span></p><p>Vova and Lesha are friends. They often meet at Vova's place and compete against each other in a computer game named The Ancient Papyri: Swordsink. Vova always chooses a warrior as his fighter and Leshac chooses an archer. After that they should choose initial positions for their characters and start the fight. A warrior is good at melee combat, so Vova will try to make the distance between fighters as small as possible. An archer prefers to keep the enemy at a distance, so Lesha will try to make the initial distance as large as possible.</p><p>There are <span class="tex-span"><i>n</i></span> (<span class="tex-span"><i>n</i></span> is always even) possible starting positions for characters marked along the <span class="tex-span"><i>Ox</i></span> axis. The positions are given by their distinct coordinates <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, two characters cannot end up at the same position.</p><p>Vova and Lesha take turns banning available positions, Vova moves first. During each turn one of the guys bans exactly one of the remaining positions. Banned positions cannot be used by <span class="tex-font-style-bf">both</span> Vova and Lesha. They continue to make moves until there are only two possible positions remaining (thus, the total number of moves will be <span class="tex-span"><i>n</i> - 2</span>). After that Vova's character takes the position with the lesser coordinate and Lesha's character takes the position with the bigger coordinate and the guys start fighting.</p><p>Vova and Lesha are already tired by the game of choosing positions, as they need to play it before every fight, so they asked you (the developer of the The Ancient Papyri: Swordsink) to write a module that would automatically determine the distance at which the warrior and the archer will start fighting if both Vova and Lesha play optimally.</p></div><div class="input-specification"><p>The first line on the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span"><i>n</i></span> is even)&nbsp;— the number of positions available initially. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), giving the coordinates of the corresponding positions.</p></div><div class="output-specification"><p>Print the distance between the warrior and the archer at the beginning of the fight, provided that both Vova and Lesha play optimally.</p></div>

## Input

<p>The first line on the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span"><i>n</i></span> is even)&nbsp;— the number of positions available initially. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), giving the coordinates of the corresponding positions.</p>

## Output

<p>Print the distance between the warrior and the archer at the beginning of the fight, provided that both Vova and Lesha play optimally.</p>





```input1
6
0 1 3 7 15 31

```




```input2
2
73 37

```




```output1
7

```




```output2
36

```



## Note

<p>In the first sample one of the optimum behavior of the players looks like that:</p><ol> <li> Vova bans the position at coordinate <span class="tex-span">15</span>; </li><li> Lesha bans the position at coordinate <span class="tex-span">3</span>; </li><li> Vova bans the position at coordinate <span class="tex-span">31</span>; </li><li> Lesha bans the position at coordinate <span class="tex-span">1</span>. </li></ol><p>After these actions only positions <span class="tex-span">0</span> and <span class="tex-span">7</span> will remain, and the distance between them is equal to <span class="tex-span">7</span>.</p><p>In the second sample there are only two possible positions, so there will be no bans.</p>
