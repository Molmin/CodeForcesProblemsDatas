## Description

<div><p>Alice and Bob play 5-in-a-row game. They have a playing field of size <span class="tex-span">10 × 10</span>. In turns they put either crosses or noughts, one at a time. Alice puts crosses and Bob puts noughts.</p><p>In current match they have made some turns and now it's Alice's turn. She wonders if she can put cross in such empty cell that she wins immediately.</p><p>Alice wins if some crosses in the field form line of length <span class="tex-font-style-bf">not smaller than <span class="tex-font-style-tt">5</span></span>. This line can be horizontal, vertical and diagonal.</p></div><div class="input-specification"><p>You are given matrix <span class="tex-span">10 × 10</span> (<span class="tex-font-style-tt">10</span> lines of <span class="tex-font-style-tt">10</span> characters each) with capital Latin letters <span class="tex-font-style-tt">'X'</span> being a cross, letters <span class="tex-font-style-tt">'O'</span> being a nought and <span class="tex-font-style-tt">'.'</span> being an empty cell. The number of <span class="tex-font-style-tt">'X'</span> cells is equal to the number of <span class="tex-font-style-tt">'O'</span> cells and there is at least one of each type. There is at least one empty cell.</p><p>It is guaranteed that in the current arrangement nobody has still won.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">'YES'</span> if it's possible for Alice to win in one turn by putting cross in some empty cell. Otherwise print <span class="tex-font-style-tt">'NO'</span>.</p></div>

## Input

<p>You are given matrix <span class="tex-span">10 × 10</span> (<span class="tex-font-style-tt">10</span> lines of <span class="tex-font-style-tt">10</span> characters each) with capital Latin letters <span class="tex-font-style-tt">'X'</span> being a cross, letters <span class="tex-font-style-tt">'O'</span> being a nought and <span class="tex-font-style-tt">'.'</span> being an empty cell. The number of <span class="tex-font-style-tt">'X'</span> cells is equal to the number of <span class="tex-font-style-tt">'O'</span> cells and there is at least one of each type. There is at least one empty cell.</p><p>It is guaranteed that in the current arrangement nobody has still won.</p>

## Output

<p>Print <span class="tex-font-style-tt">'YES'</span> if it's possible for Alice to win in one turn by putting cross in some empty cell. Otherwise print <span class="tex-font-style-tt">'NO'</span>.</p>





```input1
XX.XX.....
.....OOOO.
..........
..........
..........
..........
..........
..........
..........
..........

```




```input2
XXOXX.....
OO.O......
..........
..........
..........
..........
..........
..........
..........
..........

```




```output1
YES

```




```output2
NO

```


