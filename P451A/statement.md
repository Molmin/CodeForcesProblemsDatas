## Description

<div><p>After winning gold and silver in IOI 2014, Akshat and Malvika want to have some fun. Now they are playing a game on a grid made of <span class="tex-span"><i>n</i></span> horizontal and <span class="tex-span"><i>m</i></span> vertical sticks.</p><p>An <span class="tex-font-style-it">intersection point</span> is any point on the grid which is formed by the intersection of one horizontal stick and one vertical stick.</p><p>In the grid shown below, <span class="tex-span"><i>n</i> = 3</span> and <span class="tex-span"><i>m</i> = 3</span>. There are <span class="tex-span"><i>n</i> + <i>m</i> = 6</span> sticks in total (horizontal sticks are shown in red and vertical sticks are shown in green). There are <span class="tex-span"><i>n</i>·<i>m</i> = 9</span> intersection points, numbered from <span class="tex-span">1</span> to <span class="tex-span">9</span>.</p><center> <img class="tex-graphics" src="file://oTOJjz5y.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The rules of the game are very simple. The players move in turns. Akshat won gold, so he makes the first move. During his/her move, a player must choose any remaining intersection point and remove from the grid all sticks which pass through this point. A player will lose the game if he/she cannot make a move (i.e. there are no intersection points remaining on the grid at his/her move).</p><p>Assume that both players play optimally. Who will win the game?</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print a single line containing "<span class="tex-font-style-tt">Akshat</span>" or "<span class="tex-font-style-tt">Malvika</span>" (without the quotes), depending on the winner of the game.</p></div>

## Input

<p>The first line of input contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>).</p>

## Output

<p>Print a single line containing "<span class="tex-font-style-tt">Akshat</span>" or "<span class="tex-font-style-tt">Malvika</span>" (without the quotes), depending on the winner of the game.</p>





```input1
2 2

```




```input2
2 3

```




```input3
3 3

```




```output1
Malvika

```




```output2
Malvika

```




```output3
Akshat

```



## Note

<p><span class="tex-font-style-it">Explanation of the first sample:</span></p><p>The grid has four intersection points, numbered from <span class="tex-span">1</span> to <span class="tex-span">4</span>.</p><center> <img class="tex-graphics" src="file://jBHtGTcH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>If Akshat chooses intersection point <span class="tex-span">1</span>, then he will remove two sticks (<span class="tex-span">1 - 2</span> and <span class="tex-span">1 - 3</span>). The resulting grid will look like this.</p><center> <img class="tex-graphics" src="file://T2VZ5UXu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Now there is only one remaining intersection point (i.e. <span class="tex-span">4</span>). Malvika must choose it and remove both remaining sticks. After her move the grid will be empty.</p><p>In the empty grid, Akshat cannot make any move, hence he will lose.</p><p>Since all <span class="tex-span">4</span> intersection points of the grid are equivalent, Akshat will lose no matter which one he picks.</p>
