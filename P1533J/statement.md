## Description

<div><p>There is an infinite chessboard, divided into cells. The cell $(x, y)$ is the cell on the intersection of the $x_i$-th row and $y_i$-th column. $n$ black pawns are placed on the board, the $i$-th black pawn occupies the cell $(x_i, y_i)$.</p><p>You want to capture all black pawns. In order to do so, you may perform the following actions:</p><ul> <li> place a white pawn into any empty cell (any cell having integer coordinates can be chosen, as long as it doesn't contain any pawns); </li><li> make a move with one of the white pawns according to the chess rules. </li></ul><p>Recall that when you make a move with a white pawn in the cell $(x, y)$, the chess rules allow you to choose exactly one of these actions: </p><ul> <li> if there is a black pawn in the cell $(x + 1, y - 1)$, you can capture it — the black pawn is removed from the board, and the white pawn moves to $(x + 1, y - 1)$; </li><li> if there is a black pawn in the cell $(x + 1, y + 1)$, you can capture it — the black pawn is removed from the board, and the white pawn moves to $(x + 1, y + 1)$; </li><li> if the cell $(x + 1, y)$ is empty, you can move the white pawn to that cell. </li></ul><p>You may perform any finite sequence of actions (placing white pawns and moving them). You want to capture all of the black pawns, and it can be shown that it is always possible; and you want to do it placing as few white pawns as possible.</p><p>What is the minimum number of white pawns you have to place to capture all $n$ black pawns?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of black pawns.</p><p>Then $n$ lines follow. The $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 5 \cdot 10^5$) denoting a black pawn in the cell $(x_i, y_i)$. No cell is occupied by two or more black pawns.</p></div><div class="output-specification"><p>Print one integer — the minimum number of white pawns you have to place to capture all $n$ black pawns.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$) — the number of black pawns.</p><p>Then $n$ lines follow. The $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 5 \cdot 10^5$) denoting a black pawn in the cell $(x_i, y_i)$. No cell is occupied by two or more black pawns.</p>

## Output

<p>Print one integer — the minimum number of white pawns you have to place to capture all $n$ black pawns.</p>





```input1
3
1 1
5 1
2 2
```




```input2
3
3 2
1 3
1 1
```




```input3
2
1 1
2 2
```




```output1
1
```




```output2
2
```




```output3
1
```


