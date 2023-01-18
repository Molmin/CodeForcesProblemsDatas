## Description

<div><p>Petya and Gena play a very interesting game "Put a Knight!" on a chessboard <span class="tex-span"><i>n</i> × <i>n</i></span> in size. In this game they take turns to put chess pieces called "knights" on the board so that no two knights could threat each other. A knight located in square <span class="tex-span">(<i>r</i>, <i>c</i>)</span> can threat squares <span class="tex-span">(<i>r</i> - 1, <i>c</i> + 2)</span>, <span class="tex-span">(<i>r</i> - 1, <i>c</i> - 2)</span>, <span class="tex-span">(<i>r</i> + 1, <i>c</i> + 2)</span>, <span class="tex-span">(<i>r</i> + 1, <i>c</i> - 2)</span>, <span class="tex-span">(<i>r</i> - 2, <i>c</i> + 1)</span>, <span class="tex-span">(<i>r</i> - 2, <i>c</i> - 1)</span>, <span class="tex-span">(<i>r</i> + 2, <i>c</i> + 1)</span> and <span class="tex-span">(<i>r</i> + 2, <i>c</i> - 1)</span> (some of the squares may be located outside the chessboard). The player who can't put a new knight during his move loses. Determine which player wins considering that both players play optimally well and Petya starts.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 100</span>) — the number of boards, for which you should determine the winning player. Next <span class="tex-span"><i>T</i></span> lines contain <span class="tex-span"><i>T</i></span> integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) — the sizes of the chessboards.</p></div><div class="output-specification"><p>For each <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> × <i>n</i><sub class="lower-index"><i>i</i></sub></span> board print on a single line "<span class="tex-font-style-tt">0</span>" if Petya wins considering both players play optimally well. Otherwise, print "<span class="tex-font-style-tt">1</span>".</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 100</span>) — the number of boards, for which you should determine the winning player. Next <span class="tex-span"><i>T</i></span> lines contain <span class="tex-span"><i>T</i></span> integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) — the sizes of the chessboards.</p>

## Output

<p>For each <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> × <i>n</i><sub class="lower-index"><i>i</i></sub></span> board print on a single line "<span class="tex-font-style-tt">0</span>" if Petya wins considering both players play optimally well. Otherwise, print "<span class="tex-font-style-tt">1</span>".</p>





```input1
2
2
1

```




```output1
1
0

```


