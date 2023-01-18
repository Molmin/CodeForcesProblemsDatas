## Description

<div><p>Bashar was practicing for the national programming contest. Because of sitting too much in front of the computer without doing physical movements and eating a lot Bashar became much fatter. Bashar is going to quit programming after the national contest and he is going to become an actor (just like his father), so he should lose weight.</p><p>In order to lose weight, Bashar is going to run for $k$ kilometers. Bashar is going to run in a place that looks like a grid of $n$ rows and $m$ columns. In this grid there are two one-way roads of one-kilometer length between each pair of adjacent by side cells, one road is going from the first cell to the second one, and the other road is going from the second cell to the first one. So, there are exactly $(4 n m - 2n - 2m)$ roads.</p><p>Let's take, for example, $n = 3$ and $m = 4$. In this case, there are $34$ roads. It is the picture of this case (arrows describe roads):</p><p><img class="tex-graphics" src="file://C9NO8aHi.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Bashar wants to run by these rules:</p><ul> <li> He starts at the top-left cell in the grid; </li><li> In one move Bashar may go up (the symbol '<span class="tex-font-style-tt">U</span>'), down (the symbol '<span class="tex-font-style-tt">D</span>'), left (the symbol '<span class="tex-font-style-tt">L</span>') or right (the symbol '<span class="tex-font-style-tt">R</span>'). More formally, if he stands in the cell in the row $i$ and in the column $j$, i.e. in the cell $(i, j)$ he will move to: <ul> <li> in the case '<span class="tex-font-style-tt">U</span>' to the cell $(i-1, j)$; </li><li> in the case '<span class="tex-font-style-tt">D</span>' to the cell $(i+1, j)$; </li><li> in the case '<span class="tex-font-style-tt">L</span>' to the cell $(i, j-1)$; </li><li> in the case '<span class="tex-font-style-tt">R</span>' to the cell $(i, j+1)$; </li></ul> </li><li> He wants to run exactly $k$ kilometers, so he wants to make exactly $k$ moves; </li><li> Bashar can finish in any cell of the grid; </li><li> He can't go out of the grid so at any moment of the time he should be on some cell; </li><li> Bashar doesn't want to get bored while running so he must <span class="tex-font-style-bf">not</span> visit the same road twice. <span class="tex-font-style-bf">But he can visit the same cell any number of times</span>. </li></ul><p>Bashar asks you if it is possible to run by such rules. If it is possible, you should tell him how should he run.</p><p>You should give him $a$ steps to do and since Bashar can't remember too many steps, $a$ should not exceed $3000$. In every step, you should give him an integer $f$ and a string of moves $s$ of length at most $4$ which means that he should repeat the moves in the string $s$ for $f$ times. He will perform the steps in the order you print them.</p><p>For example, if the steps are $2$ <span class="tex-font-style-tt">RUD</span>, $3$ <span class="tex-font-style-tt">UUL</span> then the moves he is going to move are <span class="tex-font-style-tt">RUD</span> $+$ <span class="tex-font-style-tt">RUD</span> $+$ <span class="tex-font-style-tt">UUL</span> $+$ <span class="tex-font-style-tt">UUL</span> $+$ <span class="tex-font-style-tt">UUL</span> $=$ <span class="tex-font-style-tt">RUDRUDUULUULUUL</span>.</p><p>Can you help him and give him a correct sequence of moves such that the total distance he will run is equal to $k$ kilometers or say, that it is impossible?</p></div><div class="input-specification"><p>The only line contains three integers $n$, $m$ and $k$ ($1 \leq n, m \leq 500$, $1 \leq k \leq 10 ^{9}$), which are the number of rows and the number of columns in the grid and the total distance Bashar wants to run.</p></div><div class="output-specification"><p>If there is no possible way to run $k$ kilometers, print "<span class="tex-font-style-tt">NO</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line.</p><p>If the answer is "<span class="tex-font-style-tt">YES</span>", on the second line print an integer $a$ ($1 \leq a \leq 3000$)&nbsp;— the number of steps, then print $a$ lines describing the steps.</p><p>To describe a step, print an integer $f$ ($1 \leq f \leq 10^{9}$) and a string of moves $s$ of length at most $4$. Every character in $s$ should be '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">L</span>' or '<span class="tex-font-style-tt">R</span>'.</p><p>Bashar will start from the top-left cell. Make sure to move exactly $k$ moves without visiting the same road twice and without going outside the grid. <span class="tex-font-style-bf">He can finish at any cell</span>.</p><p>We can show that if it is possible to run exactly $k$ kilometers, then it is possible to describe the path under such output constraints.</p></div>

## Input

<p>The only line contains three integers $n$, $m$ and $k$ ($1 \leq n, m \leq 500$, $1 \leq k \leq 10 ^{9}$), which are the number of rows and the number of columns in the grid and the total distance Bashar wants to run.</p>

## Output

<p>If there is no possible way to run $k$ kilometers, print "<span class="tex-font-style-tt">NO</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line.</p><p>If the answer is "<span class="tex-font-style-tt">YES</span>", on the second line print an integer $a$ ($1 \leq a \leq 3000$)&nbsp;— the number of steps, then print $a$ lines describing the steps.</p><p>To describe a step, print an integer $f$ ($1 \leq f \leq 10^{9}$) and a string of moves $s$ of length at most $4$. Every character in $s$ should be '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">L</span>' or '<span class="tex-font-style-tt">R</span>'.</p><p>Bashar will start from the top-left cell. Make sure to move exactly $k$ moves without visiting the same road twice and without going outside the grid. <span class="tex-font-style-bf">He can finish at any cell</span>.</p><p>We can show that if it is possible to run exactly $k$ kilometers, then it is possible to describe the path under such output constraints.</p>





```input1
3 3 4
```




```input2
3 3 1000000000
```




```input3
3 3 8
```




```input4
4 4 9
```




```input5
3 4 16
```




```output1
YES
2
2 R
2 L
```




```output2
NO
```




```output3
YES
3
2 R
2 D
1 LLRR
```




```output4
YES
1
3 RLD
```




```output5
YES
8
3 R
3 L
1 D
3 R
1 D
1 U
3 L
1 D
```



## Note

<p>The moves Bashar is going to move in the first example are: "<span class="tex-font-style-tt">RRLL</span>".</p><p>It is not possible to run $1000000000$ kilometers in the second example because the total length of the roads is smaller and Bashar can't run the same road twice.</p><p>The moves Bashar is going to move in the third example are: "<span class="tex-font-style-tt">RRDDLLRR</span>".</p><p>The moves Bashar is going to move in the fifth example are: "<span class="tex-font-style-tt">RRRLLLDRRRDULLLD</span>". It is the picture of his run (the roads on this way are marked with red and numbered in the order of his running):</p><p><img class="tex-graphics" src="file://2AxWohub.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
