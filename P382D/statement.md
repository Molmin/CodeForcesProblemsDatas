## Description

<div><p>Ksenia has a chessboard of size <span class="tex-span"><i>n</i> × <i>m</i></span>. Each cell of the chessboard contains one of the characters: "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>", "<span class="tex-font-style-tt">^</span>", "<span class="tex-font-style-tt">v</span>", "<span class="tex-font-style-tt">#</span>". The cells that contain character "<span class="tex-font-style-tt">#</span>" are blocked. We know that all chessboard cells that touch the border are blocked.</p><p>Ksenia is playing with two pawns on this chessboard. Initially, she puts the pawns on the chessboard. One cell of the chessboard can contain two pawns if and only if the cell is blocked. In other cases two pawns can not stand in one cell. The game begins when Ksenia put pawns on the board. In one move, Ksenia moves each pawn to a side adjacent cell in the direction of arrows painted on the cell on which the corresponding pawn sits (if the pawn sits on "<span class="tex-font-style-tt">#</span>", it does not move). Assume that Ksenia moves pawns simultaneously (see the second test case). </p><p>Of course, Ksenia plays for points. How can one calculate the points per game? Very simply! Let's count how many movements the first pawn made and how many movements the second pawn made, sum these two numbers — it will be the resulting score of the game. </p><p>Ksenia wonders: what is the maximum number of points she can earn (for that, she should place the pawns optimally well early in the game). Help her and find that number. </p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2000)</span> — the sizes of the board. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters – the board's description. Each character is one of the characters: "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>", "<span class="tex-font-style-tt">^</span>", "<span class="tex-font-style-tt">v</span>", "<span class="tex-font-style-tt">#</span>".</p><p>It is guaranteed that the border cells of the table are blocked cells (with character "<span class="tex-font-style-tt">#</span>").</p></div><div class="output-specification"><p>If Ksenia can get infinitely many points, print -1. Otherwise, print the maximum number of points she can get.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2000)</span> — the sizes of the board. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters – the board's description. Each character is one of the characters: "<span class="tex-font-style-tt">&lt;</span>", "<span class="tex-font-style-tt">&gt;</span>", "<span class="tex-font-style-tt">^</span>", "<span class="tex-font-style-tt">v</span>", "<span class="tex-font-style-tt">#</span>".</p><p>It is guaranteed that the border cells of the table are blocked cells (with character "<span class="tex-font-style-tt">#</span>").</p>

## Output

<p>If Ksenia can get infinitely many points, print -1. Otherwise, print the maximum number of points she can get.</p>





```input1
1 1
#

```




```input2
3 4
####
#&gt;^{}#
####

```




```input3
3 4
####
#&gt;&lt;#
####

```




```input4
7 5
#####
##v##
##v##
#####
##^{}##
##^{}##
#####

```




```input5
7 5
#####
##v##
##v##
##&lt;##
##^{}##
##^{}##
#####
```




```output1
0

```




```output2
3
```




```output3
-1
```




```output4
4
```




```output5
5
```


