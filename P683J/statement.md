## Description

<div><p>In a new computer game you need to help the hero to get out of the maze, which is a rectangular field of size <span class="tex-span"><i>n</i> × <i>m</i></span>. The hero is located in one of the cells of this field. He knows where the exit of the maze is, and he wants to reach it.</p><p>In one move, the hero can either move to the next cell (i.e. the cell which has a common side with the current cell) if it is free, or plant a bomb on the cell where he is, or skip the move and do nothing. A planted bomb explodes after three moves, that is, after the hero makes 3 more actions but does not have time to make the fourth (all three types of moves described above are considered as actions).</p><p>The explosion destroys the obstacles in all the cells which have at least one common point with this cell (i.e. in all the cells sharing with the bomb cell a corner or a side). The explosion must not hurt the cell with the exit or the cell with the hero. The hero can not go beyond the boundaries of the maze.</p><p>Your task is to determine the sequence of hero's actions to reach the exit. Note that you haven't to minimize the length of the sequence. The only restriction — the length of the resulting sequence should not exceed 100,000 symbols.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span"><i>n</i>·<i>m</i> &gt; 1</span>) — sizes of the maze.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — description of the maze. The character "<span class="tex-font-style-tt">.</span>" means a free cell, "<span class="tex-font-style-tt">E</span>" — the hero, "<span class="tex-font-style-tt">T</span>" — the exit, "<span class="tex-font-style-tt">X</span>" — the obstacle.</p><p>It is guaranteed that there is exactly one hero and exactly one exit in the maze.</p></div><div class="output-specification"><p>Print the hero's actions which will help him get out of the maze ("<span class="tex-font-style-tt">M</span>" — to plant a bomb, "<span class="tex-font-style-tt">T</span>" — to skip the move, "<span class="tex-font-style-tt">S</span>" — to go down, "<span class="tex-font-style-tt">W</span>" — to go left, "<span class="tex-font-style-tt">N</span>" — to go up, "<span class="tex-font-style-tt">E</span>" — to go right). If the hero can not reach the exit, print "<span class="tex-font-style-tt">No solution</span>" (without quotes).</p><p>The length of the resulting sequence should not exceed 100,000 symbols. If there are several solutions it is allowed to print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>, <span class="tex-span"><i>n</i>·<i>m</i> &gt; 1</span>) — sizes of the maze.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — description of the maze. The character "<span class="tex-font-style-tt">.</span>" means a free cell, "<span class="tex-font-style-tt">E</span>" — the hero, "<span class="tex-font-style-tt">T</span>" — the exit, "<span class="tex-font-style-tt">X</span>" — the obstacle.</p><p>It is guaranteed that there is exactly one hero and exactly one exit in the maze.</p>

## Output

<p>Print the hero's actions which will help him get out of the maze ("<span class="tex-font-style-tt">M</span>" — to plant a bomb, "<span class="tex-font-style-tt">T</span>" — to skip the move, "<span class="tex-font-style-tt">S</span>" — to go down, "<span class="tex-font-style-tt">W</span>" — to go left, "<span class="tex-font-style-tt">N</span>" — to go up, "<span class="tex-font-style-tt">E</span>" — to go right). If the hero can not reach the exit, print "<span class="tex-font-style-tt">No solution</span>" (without quotes).</p><p>The length of the resulting sequence should not exceed 100,000 symbols. If there are several solutions it is allowed to print any of them.</p>





```input1
3 5
XEX.X
X.XXT
X.X.X

```




```output1
SSMNNTSSNEMWWTEEEE

```


