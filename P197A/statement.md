## Description

<div><p>You've got a rectangular table with length <span class="tex-span"><i>a</i></span> and width <span class="tex-span"><i>b</i></span> and the infinite number of plates of radius <span class="tex-span"><i>r</i></span>. Two players play the following game: they take turns to put the plates on the table so that the plates don't lie on each other (but they can touch each other), and so that any point on any plate is located within the table's border. During the game one cannot move the plates that already lie on the table. The player who cannot make another move loses. Determine which player wins, the one who moves first or the one who moves second, provided that both players play optimally well.</p></div><div class="input-specification"><p>A single line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i>, <i>r</i> ≤ 100)</span> — the table sides and the plates' radius, correspondingly.</p></div><div class="output-specification"><p>If wins the player who moves first, print "<span class="tex-font-style-tt">First</span>" (without the quotes). Otherwise print "<span class="tex-font-style-tt">Second</span>" (without the quotes).</p></div>

## Input

<p>A single line contains three space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i>, <i>r</i> ≤ 100)</span> — the table sides and the plates' radius, correspondingly.</p>

## Output

<p>If wins the player who moves first, print "<span class="tex-font-style-tt">First</span>" (without the quotes). Otherwise print "<span class="tex-font-style-tt">Second</span>" (without the quotes).</p>





```input1
5 5 2

```




```input2
6 7 4

```




```output1
First

```




```output2
Second

```



## Note

<p>In the first sample the table has place for only one plate. The first player puts a plate on the table, the second player can't do that and loses.</p><center> <img class="tex-graphics" src="file://O85Mx4S4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample the table is so small that it doesn't have enough place even for one plate. So the first player loses without making a single move.</p><center> <img class="tex-graphics" src="file://KWBdMHTf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
