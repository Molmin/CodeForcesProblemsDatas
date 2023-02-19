## Description

<div><p>Sam has been teaching Jon the <span class="tex-font-style-it">Game of Stones</span> to sharpen his mind and help him devise a strategy to fight the white walkers. The rules of this game are quite simple: </p><ul><li> The game starts with <span class="tex-span"><i>n</i></span> piles of stones indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th pile contains <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> stones.</li><li> The players make their moves alternatively. A move is considered as removal of some number of stones from a pile. Removal of <span class="tex-span">0</span> stones does not count as a move.</li><li> The player who is unable to make a move loses.</li></ul><p>Now Jon believes that he is ready for battle, but Sam does not think so. To prove his argument, Sam suggested that they play a modified version of the game.</p><p>In this modified version, no move can be made more than once on a pile. For example, if <span class="tex-span">4</span> stones are removed from a pile, <span class="tex-span">4</span> stones cannot be removed from that pile again.</p><p>Sam sets up the game and makes the first move. Jon believes that Sam is just trying to prevent him from going to battle. Jon wants to know if he can win if both play optimally.</p></div><div class="input-specification"><p>First line consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of piles.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 60</span>) — the number of stones in <span class="tex-span"><i>i</i></span>-th pile.</p></div><div class="output-specification"><p>Print a single line containing "<span class="tex-font-style-tt">YES</span>" (without quotes) if Jon wins, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes)</p></div>

## Input

<p>First line consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of piles.</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains an integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 60</span>) — the number of stones in <span class="tex-span"><i>i</i></span>-th pile.</p>

## Output

<p>Print a single line containing "<span class="tex-font-style-tt">YES</span>" (without quotes) if Jon wins, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes)</p>





```input1
1
5

```




```input2
2
1
2

```




```output1
NO
```




```output2
YES
```



## Note

<p>In the first case, Sam removes all the stones and Jon loses.</p><p>In second case, the following moves are possible by Sam: <img align="middle" class="tex-formula" src="file://jZfdAANK.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p>In each of these cases, last move can be made by Jon to win the game as follows: <img align="middle" class="tex-formula" src="file://jriOXQO9.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
