## Description

<div><p>One day Alex decided to remember childhood when computers were not too powerful and lots of people played only default games. Alex enjoyed playing Minesweeper that time. He imagined that he saved world from bombs planted by terrorists, but he rarely won.</p><p>Alex has grown up since then, so he easily wins the most difficult levels. This quickly bored him, and he thought: what if the computer gave him invalid fields in the childhood and Alex could not win because of it?</p><p>He needs your help to check it.</p><p>A Minesweeper field is a rectangle $n \times m$, where each cell is either empty, or contains a digit from $1$ to $8$, or a bomb. The field is valid if for each cell: </p><ul> <li> if there is a digit $k$ in the cell, then exactly $k$ neighboring cells have bombs. </li><li> if the cell is empty, then all neighboring cells have no bombs. </li></ul><p>Two cells are neighbors if they have a common side or a corner (i.&nbsp;e. a cell has at most $8$ neighboring cells).</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 100$) — the sizes of the field.</p><p>The next $n$ lines contain the description of the field. Each line contains $m$ characters, each of them is "<span class="tex-font-style-tt">.</span>" (if this cell is empty), "<span class="tex-font-style-tt">*</span>" (if there is bomb in this cell), or a digit from $1$ to $8$, inclusive.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>", if the field is valid and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can choose the case (lower or upper) for each letter arbitrarily.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 100$) — the sizes of the field.</p><p>The next $n$ lines contain the description of the field. Each line contains $m$ characters, each of them is "<span class="tex-font-style-tt">.</span>" (if this cell is empty), "<span class="tex-font-style-tt">*</span>" (if there is bomb in this cell), or a digit from $1$ to $8$, inclusive.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>", if the field is valid and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can choose the case (lower or upper) for each letter arbitrarily.</p>





```input1
3 3
111
1*1
111

```




```input2
2 4
*.*.
1211

```




```output1
YES
```




```output2
NO
```



## Note

<p>In the second example the answer is "<span class="tex-font-style-tt">NO</span>" because, if the positions of the bombs are preserved, the first line of the field should be <span class="tex-font-style-tt">*2*1</span>.</p><p>You can read more about Minesweeper in <a href="https://en.wikipedia.org/wiki/Minesweeper_(video_game)">Wikipedia's article</a>.</p>
