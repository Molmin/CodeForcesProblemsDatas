## Description

<div><p>Utkarsh is forced to play yet another one of Ashish's games. The game progresses turn by turn and as usual, Ashish moves <span class="tex-font-style-bf">first</span>.</p><p>Consider the 2D plane. There is a token which is initially at <span class="tex-font-style-bf">$(0,0)$</span>. In one move a player must increase either the $x$ coordinate or the $y$ coordinate of the token by <span class="tex-font-style-bf">exactly</span> $k$. In doing so, the player must ensure that the token stays within a (Euclidean) distance $d$ from $(0,0)$.</p><p>In other words, if after a move the coordinates of the token are $(p,q)$, then $p^2 + q^2 \leq d^2$ must hold.</p><p>The game ends when a player is unable to make a move. It can be shown that the game will end in a finite number of moves. If both players play optimally, determine who will win.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains two space separated integers $d$ ($1 \leq d \leq 10^5$) and $k$ ($1 \leq k \leq d$).</p></div><div class="output-specification"><p>For each test case, if Ashish wins the game, print "<span class="tex-font-style-tt">Ashish</span>", otherwise print "<span class="tex-font-style-tt">Utkarsh</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains two space separated integers $d$ ($1 \leq d \leq 10^5$) and $k$ ($1 \leq k \leq d$).</p>

## Output

<p>For each test case, if Ashish wins the game, print "<span class="tex-font-style-tt">Ashish</span>", otherwise print "<span class="tex-font-style-tt">Utkarsh</span>" (without the quotes).</p>





```input1
5
2 1
5 2
10 3
25 4
15441 33
```




```output1
Utkarsh
Ashish
Utkarsh
Utkarsh
Ashish
```



## Note

<p>In the first test case, one possible sequence of moves can be</p><p>$(0, 0) \xrightarrow{\text{Ashish }} (0, 1) \xrightarrow{\text{Utkarsh }} (0, 2)$.</p><p>Ashish has no moves left, so Utkarsh wins.</p><p><img class="tex-graphics" src="file://bDMLz9Fz.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
