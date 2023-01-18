## Description

<div><p>Alice and Bob play a game. There is a paper strip which is divided into <span class="tex-span"><i>n</i> + 1</span> cells numbered from left to right starting from <span class="tex-span">0</span>. There is a chip placed in the <span class="tex-span"><i>n</i></span>-th cell (the last one).</p><p>Players take turns, Alice is first. Each player during his or her turn has to move the chip <span class="tex-span">1</span>, <span class="tex-span">2</span> or <span class="tex-span"><i>k</i></span> cells to the left (so, if the chip is currently in the cell <span class="tex-span"><i>i</i></span>, the player can move it into cell <span class="tex-span"><i>i</i> - 1</span>, <span class="tex-span"><i>i</i> - 2</span> or <span class="tex-span"><i>i</i> - <i>k</i></span>). The chip should not leave the borders of the paper strip: it is impossible, for example, to move it <span class="tex-span"><i>k</i></span> cells to the left if the current cell has number <span class="tex-span"><i>i</i> &lt; <i>k</i></span>. The player who can't make a move loses the game.</p><p>Who wins if both participants play optimally?</p><p>Alice and Bob would like to play several games, so you should determine the winner in each game.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 100</span>) — the number of games. Next <span class="tex-span"><i>T</i></span> lines contain one game per line. All games are independent.</p><p>Each of the next <span class="tex-span"><i>T</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">3 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the length of the strip and the constant denoting the third move, respectively.</p></div><div class="output-specification"><p>For each game, print <span class="tex-font-style-tt">Alice</span> if Alice wins this game and <span class="tex-font-style-tt">Bob</span> otherwise.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 100</span>) — the number of games. Next <span class="tex-span"><i>T</i></span> lines contain one game per line. All games are independent.</p><p>Each of the next <span class="tex-span"><i>T</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">3 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the length of the strip and the constant denoting the third move, respectively.</p>

## Output

<p>For each game, print <span class="tex-font-style-tt">Alice</span> if Alice wins this game and <span class="tex-font-style-tt">Bob</span> otherwise.</p>





```input1
4
0 3
3 3
3 4
4 4

```




```output1
Bob
Alice
Bob
Alice

```


