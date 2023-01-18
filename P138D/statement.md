## Description

<div><p>Recently Roma has become the happy owner of a new game World of Darkraft. This game combines elements of virtually all known genres, and on one of the later stages of the game Roma faced difficulties solving a puzzle.</p><p>In this part Roma fights with a cunning enemy magician. The battle takes place on a rectangular field plaid <span class="tex-span"><i>n</i> × <i>m</i></span>. Each cell contains one magical character: <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span> or <span class="tex-font-style-tt">X</span>. Initially all the squares of the field are "active".</p><p>The players, Roma and enemy magician, take turns. Roma makes the first move. During a move a player selects one of the active cells. Then depending on the image in the character in the cell one of the following actions takes place: </p><ul> <li> <span class="tex-font-style-tt">L</span> — magical waves radiate from the cell to the left downwards and to the right upwards along diagonal paths. All cells on the path of the waves (including the selected cell too) become inactive. The waves continue until the next inactive cell or to the edge of the field if there are no inactive cells on the way. </li><li> <span class="tex-font-style-tt">R</span> — the magical waves radiate to the left upwards and to the right downwards. </li><li> <span class="tex-font-style-tt">X</span> — the magical waves radiate in all four diagonal directions. </li></ul><p>If the next player cannot make a move (i.e., all cells are inactive), he loses.</p><p>Roma has been trying to defeat the computer opponent for three days but he just keeps losing. He asks you to help him and determine whether it is guaranteed that he can beat the opponent, or he will have to hack the game.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters describing the playing field: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals to the magical character of the corresponding field square.</p></div><div class="output-specification"><p>On the first line print "<span class="tex-font-style-tt">WIN</span>" if Roma can win or "<span class="tex-font-style-tt">LOSE</span>" if it is impossible to win considering that the opponent pays optimally.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 20</span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters describing the playing field: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals to the magical character of the corresponding field square.</p>

## Output

<p>On the first line print "<span class="tex-font-style-tt">WIN</span>" if Roma can win or "<span class="tex-font-style-tt">LOSE</span>" if it is impossible to win considering that the opponent pays optimally.</p>





```input1
2 2
RL
LR

```




```input2
2 2
RR
RR

```




```output1
LOSE

```




```output2
WIN

```



## Note

<p>In the first test each move makes one diagonal line of the square inactive, thus it is guaranteed that Roma loses after two moves.</p><p>There are three variants of making a move in the second test: to "finish off" the main diagonal line or any of the squares that are left. That means that after three moves the game stops and Roma wins.</p>
