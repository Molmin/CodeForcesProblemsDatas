## Description

<div><p>Polycarpus has a chessboard of size <span class="tex-span"><i>n</i> × <i>m</i></span>, where <span class="tex-span"><i>k</i></span> rooks are placed. Polycarpus hasn't yet invented the rules of the game he will play. However, he has already allocated <span class="tex-span"><i>q</i></span> rectangular areas of special strategic importance on the board, they must be protected well. According to Polycarpus, a rectangular area of ​​the board is well protected if all its vacant squares can be beaten by the rooks that stand on this area. The rooks on the rest of the board do not affect the area's defense. The position of the rooks is fixed and cannot be changed. We remind you that the the rook beats the squares located on the same vertical or horizontal line with it, if there are no other pieces between the square and the rook. Help Polycarpus determine whether all strategically important areas are protected.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i>, <i>q</i> ≤ 200 000</span>) — the sizes of the board, the number of rooks and the number of strategically important sites. We will consider that the cells of the board are numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> horizontally and from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> vertically. Next <span class="tex-span"><i>k</i></span> lines contain pairs of integers "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>", describing the positions of the rooks (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span>). It is guaranteed that all the rooks are in distinct squares. Next <span class="tex-span"><i>q</i></span> lines describe the strategically important areas as groups of four integers "<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>" (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>). The corresponding rectangle area consists of cells <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, for which <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i> ≤ <i>y</i><sub class="lower-index">2</sub></span>. Strategically important areas can intersect of coincide.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. For each strategically important site print "YES" if it is well defended and "NO" otherwise.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i>, <i>q</i> ≤ 200 000</span>) — the sizes of the board, the number of rooks and the number of strategically important sites. We will consider that the cells of the board are numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> horizontally and from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> vertically. Next <span class="tex-span"><i>k</i></span> lines contain pairs of integers "<span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>", describing the positions of the rooks (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span>). It is guaranteed that all the rooks are in distinct squares. Next <span class="tex-span"><i>q</i></span> lines describe the strategically important areas as groups of four integers "<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>" (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>m</i></span>). The corresponding rectangle area consists of cells <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, for which <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i> ≤ <i>y</i><sub class="lower-index">2</sub></span>. Strategically important areas can intersect of coincide.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. For each strategically important site print "YES" if it is well defended and "NO" otherwise.</p>





```input1
4 3 3 3
1 1
3 2
2 3
2 3 2 3
2 1 3 3
1 2 2 3

```




```output1
YES
YES
NO

```



## Note

<p>Picture to the sample: <img class="tex-graphics" src="file://Mc1x7sJk.png" style="max-width: 100.0%;max-height: 100.0%;"> For the last area the answer is "NO", because cell <span class="tex-span">(1, 2)</span> cannot be hit by a rook.</p>
