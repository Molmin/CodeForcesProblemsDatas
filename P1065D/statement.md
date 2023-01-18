## Description

<div><p>You stumbled upon a new kind of chess puzzles. The chessboard you are given is not necesserily $8 \times 8$, but it still is $N \times N$. Each square has some number written on it, all the numbers are from $1$ to $N^2$ and all the numbers are pairwise distinct. The $j$-th square in the $i$-th row has a number $A_{ij}$ written on it.</p><p>In your chess set you have only three pieces: a knight, a bishop and a rook. At first, you put one of them on the square with the number $1$ (you can choose which one). Then you want to reach square $2$ (possibly passing through some other squares in process), then square $3$ and so on until you reach square $N^2$. In one step you are allowed to either make a valid move with the current piece or replace it with some other piece. <span class="tex-font-style-bf">Each square can be visited arbitrary number of times</span>.</p><p>A knight can move to a square that is two squares away horizontally and one square vertically, or two squares vertically and one square horizontally. A bishop moves diagonally. A rook moves horizontally or vertically. The move should be performed to a different square from the one a piece is currently standing on.</p><p>You want to minimize the number of steps of the whole traversal. Among all the paths to have the same number of steps you want to choose the one with the lowest number of piece replacements.</p><p>What is the path you should take to satisfy all conditions?</p></div><div class="input-specification"><p>The first line contains a single integer $N$ ($3 \le N \le 10$) — the size of the chessboard.</p><p>Each of the next $N$ lines contains $N$ integers $A_{i1}, A_{i2}, \dots, A_{iN}$ ($1 \le A_{ij} \le N^2$) — the numbers written on the squares of the $i$-th row of the board.</p><p>It is guaranteed that all $A_{ij}$ are pairwise distinct.</p></div><div class="output-specification"><p>The only line should contain two integers — the number of steps in the best answer and the number of replacement moves in it.</p></div>

## Input

<p>The first line contains a single integer $N$ ($3 \le N \le 10$) — the size of the chessboard.</p><p>Each of the next $N$ lines contains $N$ integers $A_{i1}, A_{i2}, \dots, A_{iN}$ ($1 \le A_{ij} \le N^2$) — the numbers written on the squares of the $i$-th row of the board.</p><p>It is guaranteed that all $A_{ij}$ are pairwise distinct.</p>

## Output

<p>The only line should contain two integers — the number of steps in the best answer and the number of replacement moves in it.</p>





```input1
3
1 9 3
8 6 7
4 2 5

```




```output1
12 1

```



## Note

<p>Here are the steps for the first example (the starting piece is a knight):</p><ol> <li> Move to $(3, 2)$ </li><li> Move to $(1, 3)$ </li><li> Move to $(3, 2)$ </li><li> Replace the knight with a rook </li><li> Move to $(3, 1)$ </li><li> Move to $(3, 3)$ </li><li> Move to $(3, 2)$ </li><li> Move to $(2, 2)$ </li><li> Move to $(2, 3)$ </li><li> Move to $(2, 1)$ </li><li> Move to $(1, 1)$ </li><li> Move to $(1, 2)$ </li></ol>
