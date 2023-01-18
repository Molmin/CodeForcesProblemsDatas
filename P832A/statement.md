## Description

<div><p>It's one more school day now. Sasha doesn't like classes and is always bored at them. So, each day he invents some game and plays in it alone or with friends.</p><p>Today he invented one simple game to play with Lena, with whom he shares a desk. The rules are simple. Sasha draws <span class="tex-span"><i>n</i></span> sticks in a row. After that the players take turns crossing out exactly <span class="tex-span"><i>k</i></span> sticks from left or right in each turn. Sasha moves first, because he is the inventor of the game. If there are less than <span class="tex-span"><i>k</i></span> sticks on the paper before some turn, the game ends. Sasha wins if he makes strictly more moves than Lena. Sasha wants to know the result of the game before playing, you are to help him.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of sticks drawn by Sasha and the number <span class="tex-span"><i>k</i></span>&nbsp;— the number of sticks to be crossed out on each turn.</p></div><div class="output-specification"><p>If Sasha wins, print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in arbitrary case (upper of lower).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of sticks drawn by Sasha and the number <span class="tex-span"><i>k</i></span>&nbsp;— the number of sticks to be crossed out on each turn.</p>

## Output

<p>If Sasha wins, print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in arbitrary case (upper of lower).</p>





```input1
1 1

```




```input2
10 4

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first example Sasha crosses out <span class="tex-span">1</span> stick, and then there are no sticks. So Lena can't make a move, and Sasha wins.</p><p>In the second example Sasha crosses out <span class="tex-span">4</span> sticks, then Lena crosses out <span class="tex-span">4</span> sticks, and after that there are only <span class="tex-span">2</span> sticks left. Sasha can't make a move. The players make equal number of moves, so Sasha doesn't win.</p>
