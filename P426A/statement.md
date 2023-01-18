## Description

<div><p>Sereja showed an interesting game to his friends. The game goes like that. Initially, there is a table with an empty cup and <span class="tex-span"><i>n</i></span> water mugs on it. Then all players take turns to move. During a move, a player takes a non-empty mug of water and pours all water from it into the cup. If the cup overfills, then we assume that this player lost.</p><p>As soon as Sereja's friends heard of the game, they wanted to play it. Sereja, on the other hand, wanted to find out whether his friends can play the game in such a way that there are no losers. You are given the volumes of all mugs and the cup. Also, you know that Sereja has <span class="tex-span">(<i>n</i> - 1)</span> friends. Determine if Sereja's friends can play the game so that nobody loses.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>s</i> ≤ 1000)</span> — the number of mugs and the volume of the cup. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>. Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means the volume of the <span class="tex-span"><i>i</i></span>-th mug.</p></div><div class="output-specification"><p>In a single line, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if his friends can play in the described manner, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>s</i> ≤ 1000)</span> — the number of mugs and the volume of the cup. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>. Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means the volume of the <span class="tex-span"><i>i</i></span>-th mug.</p>

## Output

<p>In a single line, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if his friends can play in the described manner, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
3 4
1 1 1

```




```input2
3 4
3 1 3

```




```input3
3 4
4 4 4

```




```output1
YES

```




```output2
YES

```




```output3
NO

```


