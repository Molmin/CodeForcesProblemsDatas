## Description

<div><p>Vasya has started watching football games. He has learned that for some fouls the players receive yellow cards, and for some fouls they receive red cards. A player who receives the second yellow card automatically receives a red card.</p><p>Vasya is watching a recorded football match now and makes notes of all the fouls that he would give a card for. Help Vasya determine all the moments in time when players would be given red cards if Vasya were the judge. For each player, Vasya wants to know only the <span class="tex-font-style-bf">first</span> moment of time when he would receive a red card from Vasya.</p></div><div class="input-specification"><p>The first line contains the name of the team playing at home. The second line contains the name of the team playing away. Both lines are not empty. The lengths of both lines do not exceed 20. Each line contains only of large English letters. The names of the teams are distinct.</p><p>Next follows number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 90</span>) — the number of fouls. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains information about a foul in the following form: </p><ul> <li> first goes number <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 90</span>) — the minute when the foul occurs; </li><li> then goes letter "<span class="tex-font-style-tt">h</span>" or letter "<span class="tex-font-style-tt">a</span>" — if the letter is "<span class="tex-font-style-tt">h</span>", then the card was given to a home team player, otherwise the card was given to an away team player; </li><li> then goes the player's number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 99</span>); </li><li> then goes letter "<span class="tex-font-style-tt">y</span>" or letter "<span class="tex-font-style-tt">r</span>" — if the letter is "<span class="tex-font-style-tt">y</span>", that means that the yellow card was given, otherwise the red card was given. </li></ul><p>The players from different teams can have the same number. The players within one team have distinct numbers. The fouls go chronologically, no two fouls happened at the same minute.</p></div><div class="output-specification"><p>For each event when a player received his first red card <span class="tex-font-style-bf">in a chronological order</span> print a string containing the following information:</p><ul> <li> The name of the team to which the player belongs; </li><li> the player's number in his team; </li><li> the minute when he received the card. </li></ul><p>If no player received a card, then you do not need to print anything.</p><p>It is possible case that the program will not print anything to the output (if there were no red cards).</p></div>

## Input

<p>The first line contains the name of the team playing at home. The second line contains the name of the team playing away. Both lines are not empty. The lengths of both lines do not exceed 20. Each line contains only of large English letters. The names of the teams are distinct.</p><p>Next follows number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 90</span>) — the number of fouls. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains information about a foul in the following form: </p><ul> <li> first goes number <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 90</span>) — the minute when the foul occurs; </li><li> then goes letter "<span class="tex-font-style-tt">h</span>" or letter "<span class="tex-font-style-tt">a</span>" — if the letter is "<span class="tex-font-style-tt">h</span>", then the card was given to a home team player, otherwise the card was given to an away team player; </li><li> then goes the player's number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 99</span>); </li><li> then goes letter "<span class="tex-font-style-tt">y</span>" or letter "<span class="tex-font-style-tt">r</span>" — if the letter is "<span class="tex-font-style-tt">y</span>", that means that the yellow card was given, otherwise the red card was given. </li></ul><p>The players from different teams can have the same number. The players within one team have distinct numbers. The fouls go chronologically, no two fouls happened at the same minute.</p>

## Output

<p>For each event when a player received his first red card <span class="tex-font-style-bf">in a chronological order</span> print a string containing the following information:</p><ul> <li> The name of the team to which the player belongs; </li><li> the player's number in his team; </li><li> the minute when he received the card. </li></ul><p>If no player received a card, then you do not need to print anything.</p><p>It is possible case that the program will not print anything to the output (if there were no red cards).</p>





```input1
MC
CSKA
9
28 a 3 y
62 h 25 y
66 h 42 y
70 h 25 y
77 a 4 y
79 a 25 y
82 h 42 r
89 h 16 y
90 a 13 r

```




```output1
MC 25 70
MC 42 82
CSKA 13 90

```


