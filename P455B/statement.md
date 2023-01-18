## Description

<div><p>Andrew, Fedor and Alex are inventive guys. Now they invent the game with strings for two players.</p><p>Given a group of <span class="tex-span"><i>n</i></span> non-empty strings. During the game two players build the word together, initially the word is empty. The players move in turns. On his step player must add a single letter in the end of the word, the resulting word must be prefix of at least one string from the group. A player loses if he cannot move.</p><p>Andrew and Alex decided to play this game <span class="tex-span"><i>k</i></span> times. The player who is the loser of the <span class="tex-span"><i>i</i></span>-th game makes the first move in the <span class="tex-span">(<i>i</i> + 1)</span>-th game. Guys decided that the winner of all games is the player who wins the last (<span class="tex-span"><i>k</i></span>-th) game. Andrew and Alex already started the game. Fedor wants to know who wins the game if both players will play optimally. Help him.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a single non-empty string from the given group. The total length of all strings from the group doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. Each string of the group consists only of lowercase English letters.</p></div><div class="output-specification"><p>If the player who moves first wins, print "<span class="tex-font-style-tt">First</span>", otherwise print "<span class="tex-font-style-tt">Second</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a single non-empty string from the given group. The total length of all strings from the group doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. Each string of the group consists only of lowercase English letters.</p>

## Output

<p>If the player who moves first wins, print "<span class="tex-font-style-tt">First</span>", otherwise print "<span class="tex-font-style-tt">Second</span>" (without the quotes).</p>





```input1
2 3
a
b

```




```input2
3 1
a
b
c

```




```input3
1 2
ab

```




```output1
First

```




```output2
First

```




```output3
Second

```


