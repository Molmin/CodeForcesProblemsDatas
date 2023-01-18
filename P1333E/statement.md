## Description

<div><p>Egor wants to achieve a rating of 1600 points on the well-known chess portal ChessForces and he needs your help!</p><p>Before you start solving the problem, Egor wants to remind you how the chess pieces move. Chess <span class="tex-font-style-bf">rook</span> moves along straight lines up and down, left and right, as many squares as it wants. And when it wants, it can stop. The <span class="tex-font-style-bf">queen</span> walks in all directions vertically and diagonally at any distance. You can see the examples below.</p><center> <img class="tex-graphics" src="file://przQ7stJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>To reach the goal, Egor should research the next topic:</p><p>There is an $N \times N$ board. Each cell of the board has a number from $1$ to $N ^ 2$ in it and numbers in all cells are distinct.</p><p>In the beginning, some chess figure stands in the cell with the number $1$. Note that this cell is already considered as visited. After that every move is determined by the following rules: </p><ol> <li> Among all <span class="tex-font-style-bf">not visited</span> yet cells to which the figure can get in one move, it goes to the cell that has <span class="tex-font-style-bf">minimal</span> number.</li><li> If all accessible cells were already visited and some cells are not yet visited, then the figure is teleported to the not visited cell that has minimal number. If this step happens, the piece pays a fee of $1$ <span class="tex-font-style-bf">vun</span>.</li><li> If all cells are already visited, the process is stopped. </li></ol><p>Egor should find an $N \times N$ board on which the rook pays <span class="tex-font-style-bf">strictly less vuns</span> than the queen during the round with this numbering. Help him to find such $N \times N$ numbered board, or tell that it doesn't exist.</p></div><div class="input-specification"><p>The only line contains one integer $N$ &nbsp;— the size of the board, $1\le N \le 500$.</p></div><div class="output-specification"><p>The output should contain $N$ lines.</p><p>In $i$-th line output $N$ numbers &nbsp;— numbers on the $i$-th row of the board. All numbers from $1$ to $N \times N$ must be used exactly once.</p><p>On your board rook must pay strictly less vuns than the queen.</p><p>If there are no solutions, print $-1$.</p><p>If there are several solutions, you can output any of them. </p></div>

## Input

<p>The only line contains one integer $N$ &nbsp;— the size of the board, $1\le N \le 500$.</p>

## Output

<p>The output should contain $N$ lines.</p><p>In $i$-th line output $N$ numbers &nbsp;— numbers on the $i$-th row of the board. All numbers from $1$ to $N \times N$ must be used exactly once.</p><p>On your board rook must pay strictly less vuns than the queen.</p><p>If there are no solutions, print $-1$.</p><p>If there are several solutions, you can output any of them. </p>





```input1
1
```




```input2
4
```




```output1
-1
```




```output2
4 3 6 12 
7 5 9 15 
14 1 11 10 
13 8 16 2
```



## Note

<p>In case we have $1 \times 1$ board, both rook and queen do not have a chance to pay fees.</p><p>In second sample <span class="tex-font-style-bf">rook</span> goes through cells $1 \to 3 \to 4 \to 6 \to 9 \to 5 \to 7 \to 13 \to 2 \to 8 \to 16 \to 11 \to 10 \to 12 \to 15 \to \textbf{(1 vun)} \to 14$. </p><p><span class="tex-font-style-bf">Queen</span> goes through $1 \to 3 \to 4 \to 2 \to 5 \to 6 \to 9 \to 7 \to 13 \to 8 \to 11 \to 10 \to 12 \to 15 \to \textbf{(1 vun)} \to 14 \to \textbf{(1 vun)} \to 16$.</p><p>As a result rook pays 1 vun and queen pays 2 vuns.</p>
