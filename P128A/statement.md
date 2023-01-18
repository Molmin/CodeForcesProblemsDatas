## Description

<div><p>In this task Anna and Maria play a game with a very unpleasant rival. Anna and Maria are in the opposite squares of a chessboard (<span class="tex-span">8 × 8</span>): Anna is in the upper right corner, and Maria is in the lower left one. Apart from them, the board has several statues. Each statue occupies exactly one square. A square that contains a statue cannot have anything or anyone — neither any other statues, nor Anna, nor Maria.</p><p>Anna is present on the board as a figurant (she stands still and never moves), and Maria has been actively involved in the game. Her goal is — to come to Anna's square. Maria and statues move in turn, Maria moves first. During one move Maria can go to any adjacent on the side or diagonal cell in which there is no statue, or she can stay in the cell where she is. The statues during their move must go one square down simultaneously, and those statues that were in the bottom row fall from the board and are no longer appeared.</p><p>At that moment, when one of the statues is in the cell in which the Maria is, the statues are declared winners. At the moment when Maria comes into the cell where Anna has been waiting, Maria is declared the winner.</p><p>Obviously, nothing depends on the statues, so it all depends on Maria. Determine who will win, if Maria does not make a strategic error.</p></div><div class="input-specification"><p>You are given the <span class="tex-span">8</span> strings whose length equals <span class="tex-span">8</span>, describing the initial position on the board. The first line represents the top row of the board, the next one — for the second from the top, and so on, the last line represents the bottom row. Each character string matches a single cell board in the appropriate row, and the characters are in the same manner as that of the corresponding cell. If the cell is empty, the corresponding character is "<span class="tex-font-style-tt">.</span>". If a cell has Maria, then it is represented by character "<span class="tex-font-style-tt">M</span>". If a cell has Anna, it is represented by the character "<span class="tex-font-style-tt">A</span>". If a cell has a statue, then the cell is represented by character "<span class="tex-font-style-tt">S</span>".</p><p>It is guaranteed that the last character of the first row is always "<span class="tex-font-style-tt">A</span>", the first character of the last line is always "<span class="tex-font-style-tt">M</span>". The remaining characters are "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">S</span>".</p></div><div class="output-specification"><p>If Maria wins, print string "<span class="tex-font-style-tt">WIN</span>". If the statues win, print string "<span class="tex-font-style-tt">LOSE</span>".</p></div>

## Input

<p>You are given the <span class="tex-span">8</span> strings whose length equals <span class="tex-span">8</span>, describing the initial position on the board. The first line represents the top row of the board, the next one — for the second from the top, and so on, the last line represents the bottom row. Each character string matches a single cell board in the appropriate row, and the characters are in the same manner as that of the corresponding cell. If the cell is empty, the corresponding character is "<span class="tex-font-style-tt">.</span>". If a cell has Maria, then it is represented by character "<span class="tex-font-style-tt">M</span>". If a cell has Anna, it is represented by the character "<span class="tex-font-style-tt">A</span>". If a cell has a statue, then the cell is represented by character "<span class="tex-font-style-tt">S</span>".</p><p>It is guaranteed that the last character of the first row is always "<span class="tex-font-style-tt">A</span>", the first character of the last line is always "<span class="tex-font-style-tt">M</span>". The remaining characters are "<span class="tex-font-style-tt">.</span>" or "<span class="tex-font-style-tt">S</span>".</p>

## Output

<p>If Maria wins, print string "<span class="tex-font-style-tt">WIN</span>". If the statues win, print string "<span class="tex-font-style-tt">LOSE</span>".</p>





```input1
.......A
........
........
........
........
........
........
M.......

```




```input2
.......A
........
........
........
........
........
SS......
M.......

```




```input3
.......A
........
........
........
........
.S......
S.......
MS......

```




```output1
WIN

```




```output2
LOSE

```




```output3
LOSE

```


