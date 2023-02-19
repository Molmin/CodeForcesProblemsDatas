## Description

<div><p>A mouse encountered a nice big cake and decided to take a walk across it, eating the berries on top of the cake on its way. The cake is rectangular, neatly divided into squares; some of the squares have a berry in them, and some don't.</p><p>The mouse is in a bit of a hurry, though, so once she enters the cake from its northwest corner (the top left cell in the input data), she will only go east (right) or south (down), until she reaches the southeast corner (the bottom right cell). She will eat every berry in the squares she passes through, but not in the other squares.</p><p>The mouse tries to choose her path so as to maximize the number of berries consumed. However, her haste and hunger might be clouding her judgement, leading her to suboptimal decisions...</p></div><div class="input-specification"><p>The first line of input contains two integers $H$ and $W$ ($1 \le H, W \le 5$), separated by a space, — the height and the width of the cake.</p><p>The next $H$ lines contain a string of $W$ characters each, representing the squares of the cake in that row: '<span class="tex-font-style-tt">.</span>' represents an empty square, and '<span class="tex-font-style-tt">*</span>' represents a square with a berry.</p></div><div class="output-specification"><p>Output the number of berries the mouse will eat following her strategy.</p></div>

## Input

<p>The first line of input contains two integers $H$ and $W$ ($1 \le H, W \le 5$), separated by a space, — the height and the width of the cake.</p><p>The next $H$ lines contain a string of $W$ characters each, representing the squares of the cake in that row: '<span class="tex-font-style-tt">.</span>' represents an empty square, and '<span class="tex-font-style-tt">*</span>' represents a square with a berry.</p>

## Output

<p>Output the number of berries the mouse will eat following her strategy.</p>





```input1
4 3
*..
.*.
..*
...
```




```input2
4 4
.*..
*...
...*
..*.
```




```input3
3 4
..**
*...
....
```




```input4
5 5
..*..
.....
**...
**...
**...
```




```output1
3
```




```output2
2
```




```output3
1
```




```output4
1
```


