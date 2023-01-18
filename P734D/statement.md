## Description

<div><p>Anton likes to play chess. Also, he likes to do programming. That is why he decided to write the program that plays chess. However, he finds the game on <span class="tex-span">8</span> to <span class="tex-span">8</span> board to too simple, he uses an infinite one instead.</p><p>The first task he faced is to check whether the king is in check. Anton doesn't know how to implement this so he asks you to help.</p><p>Consider that an infinite chess board contains one white king and the number of black pieces. There are only rooks, bishops and queens, as the other pieces are not supported yet. The white king is said to be in check if at least one black piece can reach the cell with the king in one move. </p><p>Help Anton and write the program that for the given position determines whether the white king is in check.</p><p>Remainder, on how do chess pieces move: </p><ul> <li> Bishop moves any number of cells diagonally, but it can't "leap" over the occupied cells. </li><li> Rook moves any number of cells horizontally or vertically, but it also can't "leap" over the occupied cells. </li><li> Queen is able to move any number of cells horizontally, vertically or diagonally, but it also can't "leap". </li></ul></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the number of black pieces.</p><p>The second line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the white king.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each of them contains a character and two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— type of the <span class="tex-span"><i>i</i></span>-th piece and its position. Character '<span class="tex-font-style-tt">B</span>' stands for the bishop, '<span class="tex-font-style-tt">R</span>' for the rook and '<span class="tex-font-style-tt">Q</span>' for the queen. It's guaranteed that no two pieces occupy the same position.</p></div><div class="output-specification"><p>The only line of the output should contains "<span class="tex-font-style-tt">YES</span>" (without quotes) if the white king is in check and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the number of black pieces.</p><p>The second line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">0</sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index">0</sub>, <i>y</i><sub class="lower-index">0</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the white king.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each of them contains a character and two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— type of the <span class="tex-span"><i>i</i></span>-th piece and its position. Character '<span class="tex-font-style-tt">B</span>' stands for the bishop, '<span class="tex-font-style-tt">R</span>' for the rook and '<span class="tex-font-style-tt">Q</span>' for the queen. It's guaranteed that no two pieces occupy the same position.</p>

## Output

<p>The only line of the output should contains "<span class="tex-font-style-tt">YES</span>" (without quotes) if the white king is in check and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p>





```input1
2
4 2
R 1 1
B 1 5

```




```input2
2
4 2
R 3 3
B 1 5

```




```output1
YES

```




```output2
NO

```



## Note

<p>Picture for the first sample: </p><center> <img class="tex-graphics" src="file://mxv4peh6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> White king is in check, because the black bishop can reach the cell with the white king in one move. The answer is "<span class="tex-font-style-tt">YES</span>".<p>Picture for the second sample: </p><center> <img class="tex-graphics" src="file://F4lkDN0U.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Here bishop can't reach the cell with the white king, because his path is blocked by the rook, and the bishop cant "leap" over it. Rook can't reach the white king, because it can't move diagonally. Hence, the king is not in check and the answer is "<span class="tex-font-style-tt">NO</span>".
