## Description

<div><p>Tokitsukaze is playing a game derivated from Japanese mahjong. In this game, she has three tiles in her hand. Each tile she owns is a suited tile, which means it has a suit (<span class="tex-font-style-bf">manzu</span>, <span class="tex-font-style-bf">pinzu</span> or <span class="tex-font-style-bf">souzu</span>) and a number (a digit ranged from $1$ to $9$). In this problem, we use one digit and one lowercase letter, which is the first character of the suit, to represent a suited tile. All possible suited tiles are represented as <span class="tex-font-style-tt">1m</span>, <span class="tex-font-style-tt">2m</span>, $\ldots$, <span class="tex-font-style-tt">9m</span>, <span class="tex-font-style-tt">1p</span>, <span class="tex-font-style-tt">2p</span>, $\ldots$, <span class="tex-font-style-tt">9p</span>, <span class="tex-font-style-tt">1s</span>, <span class="tex-font-style-tt">2s</span>, $\ldots$, <span class="tex-font-style-tt">9s</span>.</p><p>In order to win the game, she must have at least one <span class="tex-font-style-bf">mentsu</span> (described below) in her hand, so sometimes she should draw extra suited tiles. After drawing a tile, the number of her tiles increases by one. She can draw any tiles she wants, including those already in her hand.</p><p>Do you know the minimum number of extra suited tiles she needs to draw so that she can win?</p><p>Here are some useful definitions in this game:</p><ul> <li> A <span class="tex-font-style-bf">mentsu</span>, also known as meld, is formed by a <span class="tex-font-style-bf">koutsu</span> or a <span class="tex-font-style-bf">shuntsu</span>; </li><li> A <span class="tex-font-style-bf">koutsu</span>, also known as triplet, is made of three identical tiles, such as <span class="tex-font-style-tt">[1m, 1m, 1m]</span>, however, <span class="tex-font-style-tt">[1m, 1p, 1s]</span> or <span class="tex-font-style-tt">[1m, 4m, 7m]</span> is NOT a <span class="tex-font-style-bf">koutsu</span>; </li><li> A <span class="tex-font-style-bf">shuntsu</span>, also known as sequence, is made of three sequential numbered tiles in the same suit, such as <span class="tex-font-style-tt">[1m, 2m, 3m]</span> and <span class="tex-font-style-tt">[5s, 7s, 6s]</span>, however, <span class="tex-font-style-tt">[9m, 1m, 2m]</span> or <span class="tex-font-style-tt">[1m, 2p, 3s]</span> is NOT a <span class="tex-font-style-bf">shuntsu</span>. </li></ul><p>Some examples: </p><ul> <li> <span class="tex-font-style-tt">[2m, 3p, 2s, 4m, 1s, 2s, 4s]</span> — it contains no <span class="tex-font-style-bf">koutsu</span> or <span class="tex-font-style-bf">shuntsu</span>, so it includes no <span class="tex-font-style-bf">mentsu</span>; </li><li> <span class="tex-font-style-tt">[4s, 3m, 3p, 4s, 5p, 4s, 5p]</span> — it contains a <span class="tex-font-style-bf">koutsu</span>, <span class="tex-font-style-tt">[4s, 4s, 4s]</span>, but no <span class="tex-font-style-bf">shuntsu</span>, so it includes a <span class="tex-font-style-bf">mentsu</span>; </li><li> <span class="tex-font-style-tt">[5p, 5s, 9m, 4p, 1s, 7p, 7m, 6p]</span> — it contains no <span class="tex-font-style-bf">koutsu</span> but a <span class="tex-font-style-bf">shuntsu</span>, <span class="tex-font-style-tt">[5p, 4p, 6p]</span> or <span class="tex-font-style-tt">[5p, 7p, 6p]</span>, so it includes a <span class="tex-font-style-bf">mentsu</span>. </li></ul><p>Note that the order of tiles is unnecessary and you can assume the number of each type of suited tiles she can draw is infinite.</p></div><div class="input-specification"><p>The only line contains <span class="tex-font-style-bf">three</span> strings&nbsp;— the tiles in Tokitsukaze's hand. For each string, the first character is a digit ranged from $1$ to $9$ and the second character is <span class="tex-font-style-tt">m</span>, <span class="tex-font-style-tt">p</span> or <span class="tex-font-style-tt">s</span>.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of extra suited tiles she needs to draw.</p></div>

## Input

<p>The only line contains <span class="tex-font-style-bf">three</span> strings&nbsp;— the tiles in Tokitsukaze's hand. For each string, the first character is a digit ranged from $1$ to $9$ and the second character is <span class="tex-font-style-tt">m</span>, <span class="tex-font-style-tt">p</span> or <span class="tex-font-style-tt">s</span>.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of extra suited tiles she needs to draw.</p>





```input1
1s 2s 3s
```




```input2
9m 9m 9m
```




```input3
3p 9m 2p
```




```output1
0
```




```output2
0
```




```output3
1
```



## Note

<p>In the first example, Tokitsukaze already has a <span class="tex-font-style-bf">shuntsu</span>.</p><p>In the second example, Tokitsukaze already has a <span class="tex-font-style-bf">koutsu</span>.</p><p>In the third example, Tokitsukaze can get a <span class="tex-font-style-bf">shuntsu</span> by drawing one suited tile&nbsp;— <span class="tex-font-style-tt">1p</span> or <span class="tex-font-style-tt">4p</span>. The resulting tiles will be <span class="tex-font-style-tt">[3p, 9m, 2p, 1p]</span> or <span class="tex-font-style-tt">[3p, 9m, 2p, 4p]</span>.</p>
