## Description

<div><p>Your friend Ivan asked you to help him rearrange his desktop. The desktop can be represented as a rectangle matrix of size $n \times m$ consisting of characters '<span class="tex-font-style-tt">.</span>' (empty cell of the desktop) and '<span class="tex-font-style-tt">*</span>' (an icon).</p><p>The desktop is called <span class="tex-font-style-bf">good</span> if all its icons are occupying some prefix of full columns and, possibly, the prefix of the next column (and there are no icons outside this figure). In other words, some amount of first columns will be filled with icons and, possibly, some amount of first cells of the next (after the last full column) column will be also filled with icons (and all the icons on the desktop belong to this figure). This is pretty much the same as the real life icons arrangement.</p><p>In one move, you can take one icon and move it to any empty cell in the desktop.</p><p>Ivan loves to add some icons to his desktop and remove them from it, so he is asking you to answer $q$ queries: what is the <span class="tex-font-style-bf">minimum</span> number of moves required to make the desktop <span class="tex-font-style-bf">good</span> after adding/removing one icon?</p><p>Note that <span class="tex-font-style-bf">queries are permanent</span> and change the state of the desktop.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n$, $m$ and $q$ ($1 \le n, m \le 1000; 1 \le q \le 2 \cdot 10^5$) — the number of rows in the desktop, the number of columns in the desktop and the number of queries, respectively.</p><p>The next $n$ lines contain the description of the desktop. The $i$-th of them contains $m$ characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">*</span>' — the description of the $i$-th row of the desktop.</p><p>The next $q$ lines describe queries. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n; 1 \le y_i \le m$) — the position of the cell which changes its state (if this cell contained the icon before, then this icon is removed, otherwise an icon appears in this cell).</p></div><div class="output-specification"><p>Print $q$ integers. The $i$-th of them should be the <span class="tex-font-style-bf">minimum</span> number of moves required to make the desktop <span class="tex-font-style-bf">good</span> after applying the first $i$ queries.</p></div>

## Input

<p>The first line of the input contains three integers $n$, $m$ and $q$ ($1 \le n, m \le 1000; 1 \le q \le 2 \cdot 10^5$) — the number of rows in the desktop, the number of columns in the desktop and the number of queries, respectively.</p><p>The next $n$ lines contain the description of the desktop. The $i$-th of them contains $m$ characters '<span class="tex-font-style-tt">.</span>' and '<span class="tex-font-style-tt">*</span>' — the description of the $i$-th row of the desktop.</p><p>The next $q$ lines describe queries. The $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n; 1 \le y_i \le m$) — the position of the cell which changes its state (if this cell contained the icon before, then this icon is removed, otherwise an icon appears in this cell).</p>

## Output

<p>Print $q$ integers. The $i$-th of them should be the <span class="tex-font-style-bf">minimum</span> number of moves required to make the desktop <span class="tex-font-style-bf">good</span> after applying the first $i$ queries.</p>





```input1
4 4 8
..**
.*..
*...
...*
1 3
2 3
3 1
2 3
3 4
4 3
2 3
2 2
```




```input2
2 5 5
*...*
*****
1 3
2 2
1 3
1 5
2 3
```




```output1
3
4
4
3
4
5
5
5
```




```output2
2
3
3
3
2
```


