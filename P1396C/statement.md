## Description

<div><p>Ziota found a video game called "Monster Invaders".</p><p>Similar to every other shooting RPG game, "Monster Invaders" involves killing monsters and bosses with guns.</p><p>For the sake of simplicity, we only consider two different types of monsters and three different types of guns.</p><p>Namely, the two types of monsters are: </p><ul> <li> a normal monster with $1$ hp. </li><li> a boss with $2$ hp. </li></ul><p>And the three types of guns are: </p><ul> <li> Pistol, deals $1$ hp in damage to one monster, $r_1$ reloading time </li><li> Laser gun, deals $1$ hp in damage to all the monsters in the current level (including the boss), $r_2$ reloading time </li><li> AWP, instantly kills any monster, $r_3$ reloading time </li></ul><p><span class="tex-font-style-bf">The guns are initially not loaded, and the Ziota can only reload 1 gun at a time.</span></p><p>The levels of the game can be considered as an array $a_1, a_2, \ldots, a_n$, in which <span class="tex-font-style-bf">the $i$-th stage has $a_i$ normal monsters and 1 boss</span>. Due to the nature of the game, <span class="tex-font-style-bf">Ziota cannot use the Pistol (the first type of gun) or AWP (the third type of gun) to shoot the boss before killing all of the $a_i$ normal monsters</span>.</p><p>If Ziota damages the boss but does not kill it immediately, <span class="tex-font-style-bf">he is forced to move out of the current level to an arbitrary adjacent level</span> (adjacent levels of level $i$ $(1 &lt; i &lt; n)$ are levels $i - 1$ and $i + 1$, the only adjacent level of level $1$ is level $2$, the only adjacent level of level $n$ is level $n - 1$). Ziota can also choose to move to an adjacent level at any time. <span class="tex-font-style-bf">Each move between adjacent levels are managed by portals with $d$ teleportation time.</span></p><p>In order not to disrupt the space-time continuum within the game, <span class="tex-font-style-bf">it is strictly forbidden to reload or shoot monsters during teleportation. </span></p><p>Ziota starts the game at level 1. The objective of the game is rather simple, to kill all the bosses in all the levels. He is curious about the minimum time to finish the game (assuming it takes no time to shoot the monsters with a loaded gun and Ziota has infinite ammo on all the three guns). Please help him find this value.</p></div><div class="input-specification"><p>The first line of the input contains five integers separated by single spaces: $n$ $(2 \le n \le 10^6)$&nbsp;— the number of stages, $r_1, r_2, r_3$ $(1 \le r_1 \le r_2 \le r_3 \le 10^9)$&nbsp;— the reload time of the three guns respectively, $d$ $(1 \le d \le 10^9)$&nbsp;— the time of moving between adjacent levels.</p><p>The second line of the input contains $n$ integers separated by single spaces $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^6, 1 \le i \le n)$.</p></div><div class="output-specification"><p>Print one integer, the minimum time to finish the game.</p></div>

## Input

<p>The first line of the input contains five integers separated by single spaces: $n$ $(2 \le n \le 10^6)$&nbsp;— the number of stages, $r_1, r_2, r_3$ $(1 \le r_1 \le r_2 \le r_3 \le 10^9)$&nbsp;— the reload time of the three guns respectively, $d$ $(1 \le d \le 10^9)$&nbsp;— the time of moving between adjacent levels.</p><p>The second line of the input contains $n$ integers separated by single spaces $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^6, 1 \le i \le n)$.</p>

## Output

<p>Print one integer, the minimum time to finish the game.</p>





```input1
4 1 3 4 3
3 2 5 1
```




```input2
4 2 4 4 1
4 5 1 2
```




```output1
34
```




```output2
31
```



## Note

<p>In the first test case, the optimal strategy is:</p><ul> <li> Use the pistol to kill three normal monsters and AWP to kill the boss (Total time $1\cdot3+4=7$) </li><li> Move to stage two (Total time $7+3=10$) </li><li> Use the pistol twice and AWP to kill the boss (Total time $10+1\cdot2+4=16$) </li><li> Move to stage three (Total time $16+3=19$) </li><li> Use the laser gun and forced to move to either stage four or two, here we move to stage four (Total time $19+3+3=25$) </li><li> Use the pistol once, use AWP to kill the boss (Total time $25+1\cdot1+4=30$) </li><li> Move back to stage three (Total time $30+3=33$) </li><li> Kill the boss at stage three with the pistol (Total time $33+1=34$) </li></ul><p>Note that here, we do not finish at level $n$, but when all the bosses are killed.</p>
