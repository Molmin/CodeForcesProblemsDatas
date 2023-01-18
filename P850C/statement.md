## Description

<div><p>Mojtaba and Arpa are playing a game. They have a list of <span class="tex-span"><i>n</i></span> numbers in the game.</p><p>In a player's turn, he chooses a number <span class="tex-span"><i>p</i><sup class="upper-index"><i>k</i></sup></span> (where <span class="tex-span"><i>p</i></span> is a prime number and <span class="tex-span"><i>k</i></span> is a positive integer) such that <span class="tex-span"><i>p</i><sup class="upper-index"><i>k</i></sup></span> divides at least one number in the list. For each number in the list divisible by <span class="tex-span"><i>p</i><sup class="upper-index"><i>k</i></sup></span>, call it <span class="tex-span"><i>x</i></span>, the player will delete <span class="tex-span"><i>x</i></span> and add <img align="middle" class="tex-formula" src="file://fY7xpYiD.png" style="max-width: 100.0%;max-height: 100.0%;"> to the list. The player who can not make a valid choice of <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>k</i></span> loses.</p><p>Mojtaba starts the game and the players alternatively make moves. Determine which one of players will be the winner if both players play optimally.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of elements in the list.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the list.</p></div><div class="output-specification"><p>If Mojtaba wins, print "<span class="tex-font-style-tt">Mojtaba</span>", otherwise print "<span class="tex-font-style-tt">Arpa</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of elements in the list.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the list.</p>

## Output

<p>If Mojtaba wins, print "<span class="tex-font-style-tt">Mojtaba</span>", otherwise print "<span class="tex-font-style-tt">Arpa</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
1 1 1 1

```




```input2
4
1 1 17 17

```




```input3
4
1 1 17 289

```




```input4
5
1 2 3 4 5

```




```output1
Arpa

```




```output2
Mojtaba

```




```output3
Arpa

```




```output4
Arpa

```



## Note

<p>In the first sample test, Mojtaba can't move.</p><p>In the second sample test, Mojtaba chooses <span class="tex-span"><i>p</i> = 17</span> and <span class="tex-span"><i>k</i> = 1</span>, then the list changes to <span class="tex-span">[1, 1, 1, 1]</span>.</p><p>In the third sample test, if Mojtaba chooses <span class="tex-span"><i>p</i> = 17</span> and <span class="tex-span"><i>k</i> = 1</span>, then Arpa chooses <span class="tex-span"><i>p</i> = 17</span> and <span class="tex-span"><i>k</i> = 1</span> and wins, if Mojtaba chooses <span class="tex-span"><i>p</i> = 17</span> and <span class="tex-span"><i>k</i> = 2</span>, then Arpa chooses <span class="tex-span"><i>p</i> = 17</span> and <span class="tex-span"><i>k</i> = 1</span> and wins.</p>
