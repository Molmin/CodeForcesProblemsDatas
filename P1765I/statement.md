## Description

<div><p>The black king lives on a chess board with an infinite number of columns (files) and $8$ rows (ranks). The columns are numbered with all integer numbers (including negative). The rows are numbered from $1$ to&nbsp;$8$.</p><p>Initially, the black king is located on the starting square $(x_s, y_s)$, and he needs to reach some target square $(x_t, y_t)$. Unfortunately, there are also white pieces on the board, and they threaten the black king. After negotiations, the white pieces agreed to let the black king pass to the target square on the following conditions:</p><ul> <li> each turn, the black king makes a move according to the movement rules; </li><li> the black king cannot move to a square occupied by a white piece; </li><li> the black king cannot move to a square which is under attack by any white piece. A square is under attack if a white piece can reach it in one move according to the movement rules; </li><li> the white pieces never move. </li></ul><p>Help the black king find the minimum number of moves needed to reach the target square while not violating the conditions. The black king cannot leave the board at any time.</p><p>The black king moves according to the movement rules below. Even though the white pieces never move, squares which they can reach in one move are considered to be under attack, so the black king cannot move into those squares.</p><p>Below are the movement rules. Note that the pieces (except for the knight) cannot jump over other pieces.</p><ul> <li> a king moves exactly one square horizontally, vertically, or diagonally. </li><li> a rook moves any number of vacant squares horizontally or vertically. </li><li> a bishop moves any number of vacant squares diagonally. </li><li> a queen moves any number of vacant squares horizontally, vertically, or diagonally. </li><li> a knight moves to one of the nearest squares not on the same rank, file, or diagonal (this can be thought of as moving two squares horizontally then one square vertically, or moving one square horizontally then two squares vertically — i. e. in an "L" pattern). Knights are not blocked by other pieces, they can simply jump over them. </li></ul><p>There are no pawns on the board.</p><center> <img class="tex-graphics" src="file://NzYRvzs8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <span class="tex-font-size-small">King and knight possible moves, respectively. Dotted line shows that knight can jump over other pieces.</span> </center><center> <img class="tex-graphics" src="file://9Tf38kqB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><center> <span class="tex-font-size-small">Queen, bishop, and rook possible moves, respectively.</span> </center></div><div class="input-specification"><p>The first line contains two integers $x_s$ and $y_s$ ($1 \le x_s \le 10^8$; $1 \le y_s \le 8$) — the starting coordinates of the black king.</p><p>The second line contains two integers $x_t$ and $y_t$ ($1 \le x_t \le 10^8$; $1 \le y_t \le 8$) — the coordinates of the target square for the black king.</p><p>The third line contains one integer $n$ ($0 \le n \le 2000$) — the number of white pieces on the board.</p><p>Then $n$ lines follow, the $i$-th line contains one character $t_i$ and two integers $x_i$ and $y_i$ ($1 \le x_i \le 10^8$; $1 \le y_i \le 8$) — the type and the coordinates of the $i$-th white piece. The types of pieces are represented by the following uppercase Latin letters:</p><ul> <li> <span class="tex-font-style-tt">K</span> — king </li><li> <span class="tex-font-style-tt">Q</span> — queen </li><li> <span class="tex-font-style-tt">R</span> — rook </li><li> <span class="tex-font-style-tt">B</span> — bishop </li><li> <span class="tex-font-style-tt">N</span> — knight </li></ul><p>There can be any number of white pieces of any type listed above on the board, for example, $3$ white kings or $4$ white queens. There are no pawns on the board.</p><p>Additional constrains on the input:</p><ul> <li> no square is occupied by more than one white piece; </li><li> the starting square for the black king is different from the square he wants to reach, and neither of these two squares is occupied or is under attack by any white piece. </li></ul></div><div class="output-specification"><p>Print one integer — the minimum number of moves needed for the black king to reach the target square while not violating the conditions, or $-1$ if it is impossible.</p></div>

## Input

<p>The first line contains two integers $x_s$ and $y_s$ ($1 \le x_s \le 10^8$; $1 \le y_s \le 8$) — the starting coordinates of the black king.</p><p>The second line contains two integers $x_t$ and $y_t$ ($1 \le x_t \le 10^8$; $1 \le y_t \le 8$) — the coordinates of the target square for the black king.</p><p>The third line contains one integer $n$ ($0 \le n \le 2000$) — the number of white pieces on the board.</p><p>Then $n$ lines follow, the $i$-th line contains one character $t_i$ and two integers $x_i$ and $y_i$ ($1 \le x_i \le 10^8$; $1 \le y_i \le 8$) — the type and the coordinates of the $i$-th white piece. The types of pieces are represented by the following uppercase Latin letters:</p><ul> <li> <span class="tex-font-style-tt">K</span> — king </li><li> <span class="tex-font-style-tt">Q</span> — queen </li><li> <span class="tex-font-style-tt">R</span> — rook </li><li> <span class="tex-font-style-tt">B</span> — bishop </li><li> <span class="tex-font-style-tt">N</span> — knight </li></ul><p>There can be any number of white pieces of any type listed above on the board, for example, $3$ white kings or $4$ white queens. There are no pawns on the board.</p><p>Additional constrains on the input:</p><ul> <li> no square is occupied by more than one white piece; </li><li> the starting square for the black king is different from the square he wants to reach, and neither of these two squares is occupied or is under attack by any white piece. </li></ul>

## Output

<p>Print one integer — the minimum number of moves needed for the black king to reach the target square while not violating the conditions, or $-1$ if it is impossible.</p>





```input1
1 8
7 8
2
N 4 8
B 4 6
```




```input2
1 1
1 5
2
K 1 3
R 2 3
```




```input3
2 2
6 4
1
Q 4 3
```




```output1
10
```




```output2
6
```




```output3
-1
```



## Note

<p>The image below demonstrates the solution for the second example. Here, the letters <span class="tex-font-style-tt">K</span>, <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">s</span>, and <span class="tex-font-style-tt">t</span> represent the white king, the white rook, the starting square, and the target square, respectively. Bold crosses mark the squares which are under attack by the white pieces. Bold dots show the shortest path for the black king.</p><center> <img class="tex-graphics" src="file://oU9MKNOc.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
