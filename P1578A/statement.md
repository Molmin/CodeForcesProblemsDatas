## Description

<div><p>Let us consider the game "Sticky Tetris". In this game, there is a field of $n \times m$ squares. Tiles appear on the field and the player can move the tiles. </p><p>Each tile is a $4$-connected set of at most $7$ squares.</p><p>Each new tile appears in any position that fits inside the field, does not intersect any other tile, and the top cell of the tile is at the top row of the field. The player can move the tile left, right, and down, and at any moment the tile must still entirely fit inside the field and must not intersect other tiles. The player can stop the tile at any position at any time. After that, it cannot be moved. Since this is "Sticky Tetris," the tile will not fall once stopped.</p><p>You are given a final configuration of a "Sticky Tetris" game. You need to restore a sequence of steps that leads to that configuration if it exists.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 50$)&nbsp;— the size of the playing field.</p><p>The next $n$ lines contain a string of $m$ characters each. Each character could be either a '<span class="tex-font-style-tt">.</span>', or lowercase English letter. Connected components of the same letter correspond to a single tile. Each tile consists of at most $7$ squares.</p></div><div class="output-specification"><p>If there is no solution, print $-1$.</p><p>Otherwise, print $k$&nbsp;— the number of different tiles that are placed on the field.</p><p>On the next $k$ lines print the sequence of steps for each of the tiles in the order they are placed. </p><p>Each line consists of a number $x$ followed by a string with steps. $x$ ($1 \le x \le m$) is the starting column of the leftmost square in the top row of the tile. The string consists of characters '<span class="tex-font-style-tt">L</span>' (for left), '<span class="tex-font-style-tt">R</span>' (for right), and '<span class="tex-font-style-tt">D</span>' (for down), describing the path of that tile, ending with a single character '<span class="tex-font-style-tt">S</span>' (for stop). The final position of the tile determines which tile is being placed. The string with steps can have at most $n \cdot m + 1$ characters.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 50$)&nbsp;— the size of the playing field.</p><p>The next $n$ lines contain a string of $m$ characters each. Each character could be either a '<span class="tex-font-style-tt">.</span>', or lowercase English letter. Connected components of the same letter correspond to a single tile. Each tile consists of at most $7$ squares.</p>

## Output

<p>If there is no solution, print $-1$.</p><p>Otherwise, print $k$&nbsp;— the number of different tiles that are placed on the field.</p><p>On the next $k$ lines print the sequence of steps for each of the tiles in the order they are placed. </p><p>Each line consists of a number $x$ followed by a string with steps. $x$ ($1 \le x \le m$) is the starting column of the leftmost square in the top row of the tile. The string consists of characters '<span class="tex-font-style-tt">L</span>' (for left), '<span class="tex-font-style-tt">R</span>' (for right), and '<span class="tex-font-style-tt">D</span>' (for down), describing the path of that tile, ending with a single character '<span class="tex-font-style-tt">S</span>' (for stop). The final position of the tile determines which tile is being placed. The string with steps can have at most $n \cdot m + 1$ characters.</p>





```input1
3 2
aa
ab
aa
```




```input2
5 6
....dd
.ccccd
.cbbdd
.aab.a
aabbaa
```




```input3
5 3
...
aab
abb
aab
.bb
```




```output1
2
2 DS
1 S
```




```output2
5
2 DDDS
4 DDLS
6 DDDS
2 DS
5 S
```




```output3
-1
```


