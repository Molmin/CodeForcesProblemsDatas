## Description

<div><p>Ivan is a novice painter. He has $n$ dyes of different colors. He also knows exactly $m$ pairs of colors which harmonize with each other.</p><p>Ivan also enjoy playing chess. He has $5000$ rooks. He wants to take $k$ rooks, paint each of them in one of $n$ colors and then place this $k$ rooks on a chessboard of size $10^{9} \times 10^{9}$.</p><p>Let's call the set of rooks on the board <span class="tex-font-style-it">connected</span> if from any rook we can get to any other rook in this set moving only through cells with rooks from this set. Assume that rooks can jump over other rooks, in other words a rook can go to any cell which shares vertical and to any cell which shares horizontal.</p><p>Ivan wants his arrangement of rooks to have following properties:</p><ul><li> For any color there is a rook of this color on a board;</li><li> For any color the set of rooks of this color is connected;</li><li> For any two different colors $a$ $b$ union of set of rooks of color $a$ and set of rooks of color $b$ is connected if and only if this two colors harmonize with each other.</li></ul><p>Please help Ivan find such an arrangement.</p></div><div class="input-specification"><p>The first line of input contains $2$ integers $n$, $m$ ($1 \le n \le 100$, $0 \le m \le min(1000, \,\, \frac{n(n-1)}{2})$)&nbsp;— number of colors and number of pairs of colors which harmonize with each other.</p><p>In next $m$ lines pairs of colors which harmonize with each other are listed. Colors are numbered from $1$ to $n$. It is guaranteed that no pair occurs twice in this list.</p></div><div class="output-specification"><p>Print $n$ blocks, $i$-th of them describes rooks of $i$-th color.</p><p>In the first line of block print one number $a_{i}$ ($1 \le a_{i} \le 5000$)&nbsp;— number of rooks of color $i$. In each of next $a_{i}$ lines print two integers $x$ and $y$ ($1 \le x, \,\, y \le 10^{9}$)&nbsp;— coordinates of the next rook.</p><p>All rooks must be on different cells.</p><p>Total number of rooks must not exceed $5000$.</p><p>It is guaranteed that the solution exists.</p></div>

## Input

<p>The first line of input contains $2$ integers $n$, $m$ ($1 \le n \le 100$, $0 \le m \le min(1000, \,\, \frac{n(n-1)}{2})$)&nbsp;— number of colors and number of pairs of colors which harmonize with each other.</p><p>In next $m$ lines pairs of colors which harmonize with each other are listed. Colors are numbered from $1$ to $n$. It is guaranteed that no pair occurs twice in this list.</p>

## Output

<p>Print $n$ blocks, $i$-th of them describes rooks of $i$-th color.</p><p>In the first line of block print one number $a_{i}$ ($1 \le a_{i} \le 5000$)&nbsp;— number of rooks of color $i$. In each of next $a_{i}$ lines print two integers $x$ and $y$ ($1 \le x, \,\, y \le 10^{9}$)&nbsp;— coordinates of the next rook.</p><p>All rooks must be on different cells.</p><p>Total number of rooks must not exceed $5000$.</p><p>It is guaranteed that the solution exists.</p>





```input1
3 2
1 2
2 3

```




```input2
3 3
1 2
2 3
3 1

```




```input3
3 1
1 3

```




```output1
2
3 4
1 4
4
1 2
2 2
2 4
5 4
1
5 1

```




```output2
1
1 1
1
1 2
1
1 3

```




```output3
1
1 1
1
2 2
1
3 1

```



## Note

<p>Rooks arrangements for all three examples (red is color $1$, green is color $2$ and blue is color $3$).</p><p><img class="tex-graphics" src="file://9LpXZOLm.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img class="tex-graphics" src="file://WBZ7HBLj.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p><img class="tex-graphics" src="file://CGKsEdVh.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
