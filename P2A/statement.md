## Description

<div><p>The winner of the card game popular in Berland "Berlogging" is determined according to the following rules. If at the end of the game there is only one player with the maximum number of points, he is the winner. The situation becomes more difficult if the number of such players is more than one. During each round a player gains or loses a particular number of points. In the course of the game the number of points is registered in the line "<span class="tex-font-style-tt">name score</span>", where <span class="tex-font-style-tt">name</span> is a player's name, and <span class="tex-font-style-tt">score</span> is the number of points gained in this round, which is an integer number. If score is negative, this means that the player has lost in the round. So, if two or more players have the maximum number of points (say, it equals to <span class="tex-span"><i>m</i></span>) at the end of the game, than wins the one <span class="tex-font-style-it">of them</span> who scored at least <span class="tex-span"><i>m</i></span> points first. Initially each player has 0 points. It's guaranteed that at the end of the game at least one player has a positive number of points.</p></div><div class="input-specification"><p>The first line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  1000</span>), <span class="tex-span"><i>n</i></span> is the number of rounds played. Then follow <span class="tex-span"><i>n</i></span> lines, containing the information about the rounds in "<span class="tex-font-style-tt">name score</span>" format in chronological order, where <span class="tex-font-style-tt">name</span> is a string of lower-case Latin letters with the length from 1 to 32, and <span class="tex-font-style-tt">score</span> is an integer number between -1000 and 1000, inclusive.</p></div><div class="output-specification"><p>Print the name of the winner.</p></div>

## Input

<p>The first line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  1000</span>), <span class="tex-span"><i>n</i></span> is the number of rounds played. Then follow <span class="tex-span"><i>n</i></span> lines, containing the information about the rounds in "<span class="tex-font-style-tt">name score</span>" format in chronological order, where <span class="tex-font-style-tt">name</span> is a string of lower-case Latin letters with the length from 1 to 32, and <span class="tex-font-style-tt">score</span> is an integer number between -1000 and 1000, inclusive.</p>

## Output

<p>Print the name of the winner.</p>





```input1
3
mike 3
andrew 5
mike 2

```




```input2
3
andrew 3
andrew 2
mike 5

```




```output1
andrew

```




```output2
andrew

```


