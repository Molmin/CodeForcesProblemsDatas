## Description

<div><p>Having learned (not without some help from the Codeforces participants) to play the card game from the previous round optimally, Shrek and Donkey (as you may remember, they too live now in the Kingdom of Far Far Away) have decided to quit the boring card games and play with toy soldiers.</p><p>The rules of the game are as follows: there is a battlefield, its size equals <span class="tex-span"><i>n</i> × <i>m</i></span> squares, some squares contain the toy soldiers (the green ones belong to Shrek and the red ones belong to Donkey). Besides, each of the <span class="tex-span"><i>n</i></span> lines of the area contains not more than two soldiers. During a move a players should <span class="tex-font-style-bf">select</span> not less than <span class="tex-span">1</span> and not more than <span class="tex-span"><i>k</i></span> soldiers belonging to him and make them either <span class="tex-font-style-it">attack</span> or <span class="tex-font-style-it">retreat</span>.</p><p>An <span class="tex-font-style-it">attack</span> is moving all of the selected soldiers along the lines on which they stand <span class="tex-font-style-bf">in the direction of</span> an enemy soldier, if he is in this line. If this line doesn't have an enemy soldier, then the selected soldier on this line can move in any direction during the player's move. Each selected soldier has to move at least by one cell. Different soldiers can move by a different number of cells. During the attack the soldiers are not allowed to cross the cells where other soldiers stand (or stood immediately before the attack). It is also not allowed to go beyond the battlefield or finish the attack in the cells, where other soldiers stand (or stood immediately before attack).</p><p>A <span class="tex-font-style-it">retreat</span> is moving all of the selected soldiers along the lines on which they stand <span class="tex-font-style-bf">in the direction from</span> an enemy soldier, if he is in this line. <span class="tex-font-style-underline">The other rules repeat the rules of the attack.</span></p><p>For example, let's suppose that the original battlefield had the form (here symbols "<span class="tex-font-style-tt">G</span>" mark Shrek's green soldiers and symbols "<span class="tex-font-style-tt">R</span>" mark Donkey's red ones):</p><center> <span class="tex-font-style-tt"> <pre class="verbatim">-G-R-<br>-R-G-<br></pre> </span> </center><p>Let's suppose that <span class="tex-span"><i>k</i> = 2</span> and Shrek moves first. If he decides to <span class="tex-font-style-it">attack</span>, then after his move the battlefield can look like that:</p><center> <span class="tex-font-style-tt"> <pre class="verbatim">--GR-     --GR-     -G-R-<br>-RG--     -R-G-     -RG--<br></pre> </span> </center><p>If in the previous example Shrek decides to <span class="tex-font-style-it">retreat</span>, then after his move the battlefield can look like that:</p><center> <span class="tex-font-style-tt"> <pre class="verbatim">G--R-     G--R-     -G-R-<br>-R--G     -R-G-     -R--G<br></pre> </span> </center><p>On the other hand, the followings fields cannot result from Shrek's correct move:</p><center> <span class="tex-font-style-tt"> <pre class="verbatim">G--R-     ---RG     --GR-<br>-RG--     -R-G-     GR---<br></pre> </span> </center><p>Shrek starts the game. To make a move means to attack or to retreat by the rules. A player who cannot make a move loses and his opponent is the winner. Determine the winner of the given toy soldier game if Shrek and Donkey continue to be under the yellow pills from the last rounds' problem. Thus, they always play optimally (that is, they try to win if it is possible, or finish the game in a draw, by ensuring that it lasts forever, if they cannot win).</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100</span>). Then <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each. These characters belong to the set {"<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">R</span>"}, denoting, respectively, a battlefield's free cell, a cell occupied by Shrek's soldiers and a cell occupied by Donkey's soldiers.</p><p>It is guaranteed that each line contains no more than two soldiers.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">First</span>" (without the quotes) if Shrek wins in the given Toy Soldier game. If Donkey wins, print "<span class="tex-font-style-tt">Second</span>" (without the quotes). If the game continues forever, print "<span class="tex-font-style-tt">Draw</span>" (also without the quotes).</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100</span>). Then <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each. These characters belong to the set {"<span class="tex-font-style-tt">-</span>", "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">R</span>"}, denoting, respectively, a battlefield's free cell, a cell occupied by Shrek's soldiers and a cell occupied by Donkey's soldiers.</p><p>It is guaranteed that each line contains no more than two soldiers.</p>

## Output

<p>Print "<span class="tex-font-style-tt">First</span>" (without the quotes) if Shrek wins in the given Toy Soldier game. If Donkey wins, print "<span class="tex-font-style-tt">Second</span>" (without the quotes). If the game continues forever, print "<span class="tex-font-style-tt">Draw</span>" (also without the quotes).</p>





```input1
2 3 1
R-G
RG-

```




```input2
3 3 2
G-R
R-G
G-R

```




```input3
2 3 1
-R-
-G-

```




```input4
2 5 2
-G-R-
-R-G-

```




```output1
First

```




```output2
Second

```




```output3
Draw

```




```output4
First

```


