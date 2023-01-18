## Description

<div><p>You are given a chessboard of size <span class="tex-span">1 × <i>n</i></span>. It is guaranteed that <span class="tex-font-style-bf"><span class="tex-span"><i>n</i></span> is even</span>. The chessboard is painted like this: "<span class="tex-font-style-tt">BWBW</span><span class="tex-span">...</span><span class="tex-font-style-tt">BW</span>".</p><p>Some cells of the board are occupied by the chess pieces. Each cell contains no more than one chess piece. It is known that the total number of pieces equals to <img align="middle" class="tex-formula" src="file://dAvyK5sE.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In one step you can move one of the pieces one cell to the left or to the right. You cannot move pieces beyond the borders of the board. You also cannot move pieces to the cells that are already occupied.</p><p>Your task is to place all the pieces in the cells of the same color <span class="tex-font-style-bf">using the minimum number of moves</span> (all the pieces must occupy only the black cells or only the white cells after all the moves are made).</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-font-style-bf"><span class="tex-span"><i>n</i></span> is even</span>) — the size of the chessboard. </p><p>The second line of the input contains <img align="middle" class="tex-formula" src="file://nEU49glH.png" style="max-width: 100.0%;max-height: 100.0%;"> integer numbers <img align="middle" class="tex-formula" src="file://exKTNXfZ.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — initial positions of the pieces. It is guaranteed that all the positions are distinct.</p></div><div class="output-specification"><p>Print one integer — <span class="tex-font-style-bf">the minimum number of moves</span> you have to make to place all the pieces in the cells of the same color.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-font-style-bf"><span class="tex-span"><i>n</i></span> is even</span>) — the size of the chessboard. </p><p>The second line of the input contains <img align="middle" class="tex-formula" src="file://nEU49glH.png" style="max-width: 100.0%;max-height: 100.0%;"> integer numbers <img align="middle" class="tex-formula" src="file://exKTNXfZ.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — initial positions of the pieces. It is guaranteed that all the positions are distinct.</p>

## Output

<p>Print one integer — <span class="tex-font-style-bf">the minimum number of moves</span> you have to make to place all the pieces in the cells of the same color.</p>





```input1
6
1 2 6

```




```input2
10
1 2 3 4 5

```




```output1
2

```




```output2
10

```



## Note

<p>In the first example the only possible strategy is to move the piece at the position <span class="tex-span">6</span> to the position <span class="tex-span">5</span> and move the piece at the position <span class="tex-span">2</span> to the position <span class="tex-span">3</span>. Notice that if you decide to place the pieces in the white cells the minimum number of moves will be <span class="tex-span">3</span>.</p><p>In the second example the possible strategy is to move <img align="middle" class="tex-formula" src="file://5D2z7INi.png" style="max-width: 100.0%;max-height: 100.0%;"> in 4 moves, then <img align="middle" class="tex-formula" src="file://9aA5Vmoj.png" style="max-width: 100.0%;max-height: 100.0%;"> in 3 moves, <img align="middle" class="tex-formula" src="file://J11bUuw8.png" style="max-width: 100.0%;max-height: 100.0%;"> in 2 moves and <img align="middle" class="tex-formula" src="file://Xi0kV2Ph.png" style="max-width: 100.0%;max-height: 100.0%;"> in 1 move.</p>
