## Description

<div><p>Vasya has been playing Plane of Tanks with his friends the whole year. Now it is time to divide the participants into several categories depending on their results. </p><p>A player is given a non-negative integer number of points in each round of the Plane of Tanks. Vasya wrote results for each round of the last year. He has <span class="tex-span"><i>n</i></span> records in total.</p><p>In order to determine a player's category consider the best result obtained by the player and the best results of other players. The player belongs to category: </p><ul> <li> "<span class="tex-font-style-tt">noob</span>" — if <span class="tex-font-style-bf">more than <span class="tex-span">50%</span> of players have better results</span>; </li><li> "<span class="tex-font-style-tt">random</span>" — if his result is not worse than the result that <span class="tex-span">50%</span> of players have, but more than <span class="tex-span">20%</span> of players have better results; </li><li> "<span class="tex-font-style-tt">average</span>" — if his result is not worse than the result that <span class="tex-span">80%</span> of players have, but more than <span class="tex-span">10%</span> of players have better results; </li><li> "<span class="tex-font-style-tt">hardcore</span>" — if his result is not worse than the result that <span class="tex-span">90%</span> of players have, but more than <span class="tex-span">1%</span> of players have better results; </li><li> "<span class="tex-font-style-tt">pro</span>" — if his result is not worse than the result that <span class="tex-span">99%</span> of players have. </li></ul> <p>When the percentage is calculated the player himself is taken into account. That means that if two players played the game and the first one gained 100 points and the second one 1000 points, then the first player's result is not worse than the result that <span class="tex-span">50%</span> of players have, and the second one is not worse than the result that <span class="tex-span">100%</span> of players have.</p><p>Vasya gave you the last year Plane of Tanks results. Help Vasya determine each player's category.</p></div><div class="input-specification"><p>The first line contains the only integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — a number of records with the players' results.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a player's name and the amount of points, obtained by the player for the round, separated with a space. The name contains not less than 1 and no more than 10 characters. The name consists of lowercase Latin letters only. It is guaranteed that any two different players have different names. The amount of points, obtained by the player for the round, is a non-negative integer number and does not exceed 1000.</p></div><div class="output-specification"><p>Print on the first line the number <span class="tex-span"><i>m</i></span> — the number of players, who participated in one round at least.</p><p>Each one of the next <span class="tex-span"><i>m</i></span> lines should contain a player name and a category he belongs to, separated with space. Category can be one of the following: "<span class="tex-font-style-tt">noob</span>", "<span class="tex-font-style-tt">random</span>", "<span class="tex-font-style-tt">average</span>", "<span class="tex-font-style-tt">hardcore</span>" or "<span class="tex-font-style-tt">pro</span>" (without quotes). The name of each player should be printed only once. Player names with respective categories can be printed in an arbitrary order.</p></div>

## Input

<p>The first line contains the only integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — a number of records with the players' results.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a player's name and the amount of points, obtained by the player for the round, separated with a space. The name contains not less than 1 and no more than 10 characters. The name consists of lowercase Latin letters only. It is guaranteed that any two different players have different names. The amount of points, obtained by the player for the round, is a non-negative integer number and does not exceed 1000.</p>

## Output

<p>Print on the first line the number <span class="tex-span"><i>m</i></span> — the number of players, who participated in one round at least.</p><p>Each one of the next <span class="tex-span"><i>m</i></span> lines should contain a player name and a category he belongs to, separated with space. Category can be one of the following: "<span class="tex-font-style-tt">noob</span>", "<span class="tex-font-style-tt">random</span>", "<span class="tex-font-style-tt">average</span>", "<span class="tex-font-style-tt">hardcore</span>" or "<span class="tex-font-style-tt">pro</span>" (without quotes). The name of each player should be printed only once. Player names with respective categories can be printed in an arbitrary order.</p>





```input1
5
vasya 100
vasya 200
artem 100
kolya 200
igor 250

```




```input2
3
vasya 200
kolya 1000
vasya 1000

```




```output1
4
artem noob
igor pro
kolya random
vasya random

```




```output2
2
kolya pro
vasya pro

```



## Note

<p>In the first example the best result, obtained by <span class="tex-font-style-tt">artem</span> is not worse than the result that <span class="tex-span">25%</span> of players have (his own result), so he belongs to category "<span class="tex-font-style-tt">noob</span>". <span class="tex-font-style-tt">vasya</span> and <span class="tex-font-style-tt">kolya</span> have best results not worse than the results that <span class="tex-span">75%</span> players have (both of them and <span class="tex-font-style-tt">artem</span>), so they belong to category "<span class="tex-font-style-tt">random</span>". <span class="tex-font-style-tt">igor</span> has best result not worse than the result that <span class="tex-span">100%</span> of players have (all other players and himself), so he belongs to category "<span class="tex-font-style-tt">pro</span>".</p><p>In the second example both players have the same amount of points, so they have results not worse than <span class="tex-span">100%</span> players have, so they belong to category "<span class="tex-font-style-tt">pro</span>".</p>
