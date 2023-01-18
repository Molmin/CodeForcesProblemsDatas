## Description

<div><p>Once Volodya was at the museum and saw a regular chessboard as a museum piece. And there were only four chess pieces on it: two white rooks, a white king and a black king. "Aha, blacks certainly didn't win!", — Volodya said and was right for sure. And your task is to say whether whites had won or not.</p><p>Pieces on the chessboard are guaranteed to represent a correct position (every piece occupies one cell, no two pieces occupy the same cell and kings cannot take each other). Thus, your task is only to decide whether whites mate blacks. We would remind you that it means that the black king can be taken by one of the opponent's pieces at the moment and also it cannot move to an unbeaten position. A rook moves vertically or horizontally by any number of <span class="tex-font-style-it">free</span> cells (assuming there are no other pieces on its path), a king — to the adjacent cells (either by corner or by side). Certainly, pieces cannot leave the board. The black king might be able to take opponent's rooks at his turn (see sample 3).</p></div><div class="input-specification"><p>The input contains 4 space-separated piece positions: positions of the two rooks, the white king and the black king. Each position on <span class="tex-span">8 × 8</span> chessboard is denoted by two symbols — (<span class="tex-font-style-tt">'a'</span> - <span class="tex-font-style-tt">'h'</span>) and (<span class="tex-font-style-tt">'1'</span> - <span class="tex-font-style-tt">'8'</span>) — which stand for horizontal and vertical coordinates of the cell occupied by the piece. It is guaranteed, that no two pieces occupy the same cell, and kings cannot take each other.</p></div><div class="output-specification"><p>Output should contain one word: <span class="tex-font-style-tt">"CHECKMATE"</span> if whites mate blacks, and <span class="tex-font-style-tt">"OTHER"</span> otherwise.</p></div>

## Input

<p>The input contains 4 space-separated piece positions: positions of the two rooks, the white king and the black king. Each position on <span class="tex-span">8 × 8</span> chessboard is denoted by two symbols — (<span class="tex-font-style-tt">'a'</span> - <span class="tex-font-style-tt">'h'</span>) and (<span class="tex-font-style-tt">'1'</span> - <span class="tex-font-style-tt">'8'</span>) — which stand for horizontal and vertical coordinates of the cell occupied by the piece. It is guaranteed, that no two pieces occupy the same cell, and kings cannot take each other.</p>

## Output

<p>Output should contain one word: <span class="tex-font-style-tt">"CHECKMATE"</span> if whites mate blacks, and <span class="tex-font-style-tt">"OTHER"</span> otherwise.</p>





```input1
a6 b4 c8 a8

```




```input2
a6 c4 b6 b8

```




```input3
a2 b1 a3 a1

```




```output1
CHECKMATE

```




```output2
OTHER

```




```output3
OTHER

```


