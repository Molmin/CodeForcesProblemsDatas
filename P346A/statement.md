## Description

<div><p>It is so boring in the summer holiday, isn't it? So Alice and Bob have invented a new game to play. The rules are as follows. First, they get a set of <span class="tex-span"><i>n</i></span> distinct integers. And then they take turns to make the following moves. During each move, either Alice or Bob (the player whose turn is the current) can choose two distinct integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> from the set, such that the set doesn't contain their absolute difference <span class="tex-span">|<i>x</i> - <i>y</i>|</span>. Then this player adds integer <span class="tex-span">|<i>x</i> - <i>y</i>|</span> to the set (so, the size of the set increases by one).</p><p>If the current player has no valid move, he (or she) loses the game. The question is who will finally win the game if both players play optimally. Remember that Alice always moves first.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the initial number of elements in the set. The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the set.</p></div><div class="output-specification"><p>Print a single line with the winner's name. If Alice wins print "<span class="tex-font-style-tt">Alice</span>", otherwise print "<span class="tex-font-style-tt">Bob</span>" (without quotes).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) — the initial number of elements in the set. The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the set.</p>

## Output

<p>Print a single line with the winner's name. If Alice wins print "<span class="tex-font-style-tt">Alice</span>", otherwise print "<span class="tex-font-style-tt">Bob</span>" (without quotes).</p>





```input1
2
2 3

```




```input2
2
5 3

```




```input3
3
5 6 7

```




```output1
Alice

```




```output2
Alice

```




```output3
Bob

```



## Note

<p>Consider the first test sample. Alice moves first, and the only move she can do is to choose 2 and 3, then to add 1 to the set. Next Bob moves, there is no valid move anymore, so the winner is Alice.</p>
