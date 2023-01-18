## Description

<div><p>A queen is the strongest chess piece. In modern chess the queen can move any number of squares in any horizontal, vertical or diagonal direction (considering that there're no other pieces on its way). The queen combines the options given to the rook and the bishop.</p><p>There are <span class="tex-span"><i>m</i></span> queens on a square <span class="tex-span"><i>n</i> × <i>n</i></span> chessboard. You know each queen's positions, the <span class="tex-span"><i>i</i></span>-th queen is positioned in the square <span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>)</span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> is the board row number (numbered from the top to the bottom from 1 to <span class="tex-span"><i>n</i></span>), and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the board's column number (numbered from the left to the right from 1 to <span class="tex-span"><i>n</i></span>). No two queens share the same position.</p><p>For each queen one can count <span class="tex-span"><i>w</i></span> — the number of other queens that the given queen threatens (attacks). For a fixed attack direction only the first queen in this direction is under attack if there are many queens are on the ray of the attack. Obviously, for any queen <span class="tex-span"><i>w</i></span> is between 0 and 8, inclusive.</p><p>Print the sequence <span class="tex-span"><i>t</i><sub class="lower-index">0</sub>, <i>t</i><sub class="lower-index">1</sub>, ..., <i>t</i><sub class="lower-index">8</sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the number of queens that threaten exactly <span class="tex-span"><i>i</i></span> other queens, i.e. the number of queens that their <span class="tex-span"><i>w</i></span> equals <span class="tex-span"><i>i</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains a pair of integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the size of the board and <span class="tex-span"><i>m</i></span> is the number of queens on the board. Then <span class="tex-span"><i>m</i></span> following lines contain positions of the queens, one per line. Each line contains a pair of integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the queen's position. No two queens stand on the same square.</p></div><div class="output-specification"><p>Print the required sequence <span class="tex-span"><i>t</i><sub class="lower-index">0</sub>, <i>t</i><sub class="lower-index">1</sub>, ..., <i>t</i><sub class="lower-index">8</sub></span>, separating the numbers with spaces.</p></div>

## Input

<p>The first line of the input contains a pair of integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the size of the board and <span class="tex-span"><i>m</i></span> is the number of queens on the board. Then <span class="tex-span"><i>m</i></span> following lines contain positions of the queens, one per line. Each line contains a pair of integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the queen's position. No two queens stand on the same square.</p>

## Output

<p>Print the required sequence <span class="tex-span"><i>t</i><sub class="lower-index">0</sub>, <i>t</i><sub class="lower-index">1</sub>, ..., <i>t</i><sub class="lower-index">8</sub></span>, separating the numbers with spaces.</p>





```input1
8 4
4 3
4 8
6 5
1 6

```




```input2
10 3
1 1
1 2
1 3

```




```output1
0 3 0 1 0 0 0 0 0
```




```output2
0 2 1 0 0 0 0 0 0
```


