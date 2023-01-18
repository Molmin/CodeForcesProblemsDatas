## Description

<div><p>There is an infinite board of square tiles. Initially all tiles are white.</p><p>Vova has a red marker and a blue marker. Red marker can color $a$ tiles. Blue marker can color $b$ tiles. If some tile isn't white then you can't use marker of any color on it. Each marker must be drained completely, so at the end there should be exactly $a$ red tiles and exactly $b$ blue tiles across the board.</p><p>Vova wants to color such a set of tiles that:</p><ul> <li> they would form a <span class="tex-font-style-bf">rectangle</span>, consisting of exactly $a+b$ colored tiles; </li><li> all tiles of at least one color would also form a <span class="tex-font-style-bf">rectangle</span>. </li></ul><p>Here are some examples of correct colorings:</p><center> <img class="tex-graphics" src="file://wO0cdgAY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Here are some examples of incorrect colorings:</p><center> <img class="tex-graphics" src="file://4dRnyBNE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Among all correct colorings Vova wants to choose the one with the minimal perimeter. What is the minimal perimeter Vova can obtain?</p><p>It is guaranteed that there exists at least one correct coloring.</p></div><div class="input-specification"><p>A single line contains two integers $a$ and $b$ ($1 \le a, b \le 10^{14}$) — the number of tiles red marker should color and the number of tiles blue marker should color, respectively.</p></div><div class="output-specification"><p>Print a single integer — the minimal perimeter of a colored rectangle Vova can obtain by coloring exactly $a$ tiles red and exactly $b$ tiles blue.</p><p>It is guaranteed that there exists at least one correct coloring.</p></div>

## Input

<p>A single line contains two integers $a$ and $b$ ($1 \le a, b \le 10^{14}$) — the number of tiles red marker should color and the number of tiles blue marker should color, respectively.</p>

## Output

<p>Print a single integer — the minimal perimeter of a colored rectangle Vova can obtain by coloring exactly $a$ tiles red and exactly $b$ tiles blue.</p><p>It is guaranteed that there exists at least one correct coloring.</p>





```input1
4 4

```




```input2
3 9

```




```input3
9 3

```




```input4
3 6

```




```input5
506 2708

```




```output1
12

```




```output2
14

```




```output3
14

```




```output4
12

```




```output5
3218

```



## Note

<p>The first four examples correspond to the first picture of the statement.</p><p>Note that for there exist multiple correct colorings for all of the examples.</p><p>In the first example you can also make a rectangle with sides $1$ and $8$, though its perimeter will be $18$ which is greater than $8$.</p><p>In the second example you can make the same resulting rectangle with sides $3$ and $4$, but red tiles will form the rectangle with sides $1$ and $3$ and blue tiles will form the rectangle with sides $3$ and $3$.</p>
