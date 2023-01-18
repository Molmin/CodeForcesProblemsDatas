## Description

<div><p>Tavas lives in Kansas. Kansas has <span class="tex-span"><i>n</i></span> cities numbered from 1 to <span class="tex-span"><i>n</i></span> connected with <span class="tex-span"><i>m</i></span> bidirectional roads. We can travel from any city to any other city via these roads. Kansas is as strange as Tavas. So there may be a road between a city and itself or more than one road between two cities.</p><p>Tavas invented a game and called it "Dashti". He wants to play Dashti with his girlfriends, Nafas.</p><p>In this game, they assign an arbitrary integer value to each city of Kansas. The value of <span class="tex-span"><i>i</i></span>-th city equals to <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>During the game, Tavas is in city <span class="tex-span"><i>s</i></span> and Nafas is in city <span class="tex-span"><i>t</i></span>. They play in turn and Tavas goes first. A player in his/her turn, must choose a non-negative integer <span class="tex-span"><i>x</i></span> and his/her score increases by the sum of values of all cities with (shortest) distance no more than <span class="tex-span"><i>x</i></span> from his/her city. Each city may be used once, or in the other words, after first time a player gets score from a city, city score becomes zero.</p><p>There is an additional rule: the player must choose <span class="tex-span"><i>x</i></span> such that he/she gets the point of at least one city that was not used before. Note that city may initially have value 0, such city isn't considered as been used at the beginning of the game, i. e. each player may use it to fullfill this rule.</p><p>The game ends when nobody can make a move.</p><p>A player's score is the sum of the points he/she earned during the game. The winner is the player with greater score, or there is a draw if players score the same value. Both players start game with zero points.</p><center> <img class="tex-graphics" src="file://fU77rQp0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If Tavas wins, he'll break his girlfriend's heart, and if Nafas wins, Tavas will cry. But if their scores are equal, they'll be happy and Tavas will give Nafas flowers.</p><p>They're not too emotional after all, so they'll play optimally. Your task is to tell Tavas what's going to happen after the game ends.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line of input contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i> ≠ <i>t</i></span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">|<i>p</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the roads. Each line contains three integers <span class="tex-span"><i>v</i>, <i>u</i>, <i>w</i></span> and it means that there's an road with length <span class="tex-span"><i>w</i></span> between cities <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span> and <span class="tex-span">0 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>). The road may lead from the city to itself, there may be several roads between each pair of cities.</p></div><div class="output-specification"><p>If Tavas wins, print "<span class="tex-font-style-tt">Break a heart</span>". If Nafas wins print "<span class="tex-font-style-tt">Cry</span>" and if nobody wins (i. e. the game ended with draw) print "<span class="tex-font-style-tt">Flowers</span>".</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line of input contains two integers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i> ≠ <i>t</i></span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> separated by spaces (<span class="tex-span">|<i>p</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the roads. Each line contains three integers <span class="tex-span"><i>v</i>, <i>u</i>, <i>w</i></span> and it means that there's an road with length <span class="tex-span"><i>w</i></span> between cities <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span> and <span class="tex-span">0 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>). The road may lead from the city to itself, there may be several roads between each pair of cities.</p>

## Output

<p>If Tavas wins, print "<span class="tex-font-style-tt">Break a heart</span>". If Nafas wins print "<span class="tex-font-style-tt">Cry</span>" and if nobody wins (i. e. the game ended with draw) print "<span class="tex-font-style-tt">Flowers</span>".</p>





```input1
4 4
1 2
3 2 5 -11
1 4 2
3 4 2
3 1 5
3 2 1

```




```input2
5 4
1 2
2 2 -5 -4 6
1 2 4
2 3 5
2 4 2
4 5 2

```




```input3
2 1
1 2
-5 -5
1 2 10

```




```output1
Cry

```




```output2
Break a heart

```




```output3
Flowers

```


