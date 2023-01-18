## Description

<div><p>On some square in the lowest row of a chessboard a stands a pawn. It has only two variants of moving: upwards and leftwards or upwards and rightwards. The pawn can choose from which square of the lowest row it can start its journey. On each square lay from 0 to 9 peas. The pawn wants to reach the uppermost row having collected as many peas as possible. As there it will have to divide the peas between itself and its <span class="tex-span"><i>k</i></span> brothers, the number of peas must be divisible by <span class="tex-span"><i>k</i> + 1</span>. Find the maximal number of peas it will be able to collect and which moves it should make to do it.</p><p>The pawn cannot throw peas away or leave the board. When a pawn appears in some square of the board (including the first and last square of the way), it necessarily takes all the peas.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100, 0 ≤ <i>k</i> ≤ 10</span>) — the number of rows and columns on the chessboard, the number of the pawn's brothers. Then follow <span class="tex-span"><i>n</i></span> lines containing each <span class="tex-span"><i>m</i></span> numbers from 0 to 9 without spaces — the chessboard's description. Each square is described by one number — the number of peas in it. The first line corresponds to the uppermost row and the last line — to the lowest row.</p></div><div class="output-specification"><p>If it is impossible to reach the highest row having collected the number of peas divisible by <span class="tex-span"><i>k</i> + 1</span>, print <span class="tex-font-style-tt">-1</span>. </p><p>Otherwise, the first line must contain a single number — the maximal number of peas the pawn can collect given that the number must be divisible by <span class="tex-span"><i>k</i> + 1</span>. The second line must contain a single number — the number of the square's column in the lowest row, from which the pawn must start its journey. The columns are numbered from the left to the right with integral numbers starting from <span class="tex-span">1</span>. The third line must contain a line consisting of <span class="tex-span"><i>n</i> - 1</span> symbols — the description of the pawn's moves. If the pawn must move upwards and leftwards, print <span class="tex-font-style-tt">L</span>, if it must move upwards and rightwards, print <span class="tex-font-style-tt">R</span>. If there are several solutions to that problem, print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 100, 0 ≤ <i>k</i> ≤ 10</span>) — the number of rows and columns on the chessboard, the number of the pawn's brothers. Then follow <span class="tex-span"><i>n</i></span> lines containing each <span class="tex-span"><i>m</i></span> numbers from 0 to 9 without spaces — the chessboard's description. Each square is described by one number — the number of peas in it. The first line corresponds to the uppermost row and the last line — to the lowest row.</p>

## Output

<p>If it is impossible to reach the highest row having collected the number of peas divisible by <span class="tex-span"><i>k</i> + 1</span>, print <span class="tex-font-style-tt">-1</span>. </p><p>Otherwise, the first line must contain a single number — the maximal number of peas the pawn can collect given that the number must be divisible by <span class="tex-span"><i>k</i> + 1</span>. The second line must contain a single number — the number of the square's column in the lowest row, from which the pawn must start its journey. The columns are numbered from the left to the right with integral numbers starting from <span class="tex-span">1</span>. The third line must contain a line consisting of <span class="tex-span"><i>n</i> - 1</span> symbols — the description of the pawn's moves. If the pawn must move upwards and leftwards, print <span class="tex-font-style-tt">L</span>, if it must move upwards and rightwards, print <span class="tex-font-style-tt">R</span>. If there are several solutions to that problem, print any of them.</p>





```input1
3 3 1
123
456
789

```




```input2
3 3 0
123
456
789

```




```input3
2 2 10
98
75

```




```output1
16
2
RL

```




```output2
17
3
LR

```




```output3
-1

```


