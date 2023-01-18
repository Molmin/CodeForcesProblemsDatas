## Description

<div><p>President of Berland has a very vast office-room, where, apart from him, work his subordinates. Each subordinate, as well as President himself, has his own desk of a unique colour. Each desk is rectangular, and its sides are parallel to the office walls. One day President decided to establish an assembly, of which all his deputies will be members. Unfortunately, he does not remember the exact amount of his deputies, but he remembers that the desk of each his deputy is adjacent to his own desk, that is to say, the two desks (President's and each deputy's) have a common side of a positive length.</p><p>The office-room plan can be viewed as a matrix with <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. Each cell of this matrix is either empty, or contains a part of a desk. An uppercase Latin letter stands for each desk colour. The «period» character («<span class="tex-font-style-tt">.</span>») stands for an empty cell. </p></div><div class="input-specification"><p>The first line contains two separated by a space integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the length and the width of the office-room, and <span class="tex-span"><i>c</i></span> character — the President's desk colour. The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the office-room description. It is guaranteed that the colour of each desk is unique, and each desk represents a continuous subrectangle of the given matrix. All colours are marked by uppercase Latin letters.</p></div><div class="output-specification"><p>Print the only number — the amount of President's deputies.</p></div>

## Input

<p>The first line contains two separated by a space integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the length and the width of the office-room, and <span class="tex-span"><i>c</i></span> character — the President's desk colour. The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each — the office-room description. It is guaranteed that the colour of each desk is unique, and each desk represents a continuous subrectangle of the given matrix. All colours are marked by uppercase Latin letters.</p>

## Output

<p>Print the only number — the amount of President's deputies.</p>





```input1
3 4 R
G.B.
.RR.
TTT.

```




```input2
3 3 Z
...
.H.
..Z

```




```output1
2

```




```output2
0

```


