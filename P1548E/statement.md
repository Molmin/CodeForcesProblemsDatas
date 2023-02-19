## Description

<div><p>Two painters, Amin and Benj, are repainting Gregor's living room ceiling! The ceiling can be modeled as an $n \times m$ grid.</p><p>For each $i$ between $1$ and $n$, inclusive, painter Amin applies $a_i$ layers of paint to the entire $i$-th row. For each $j$ between $1$ and $m$, inclusive, painter Benj applies $b_j$ layers of paint to the entire $j$-th column. Therefore, the cell $(i,j)$ ends up with $a_i+b_j$ layers of paint.</p><p>Gregor considers the cell $(i,j)$ to be <span class="tex-font-style-it">badly painted</span> if $a_i+b_j \le x$. Define a <span class="tex-font-style-it">badly painted region</span> to be a <span class="tex-font-style-bf">maximal</span> connected component of badly painted cells, i.&nbsp;e. a connected component of badly painted cells such that all adjacent to the component cells are not badly painted. Two cells are considered adjacent if they share a side.</p><p>Gregor is appalled by the state of the finished ceiling, and wants to know the number of badly painted regions.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $x$ ($1 \le n,m \le 2\cdot 10^5$, $1 \le x \le 2\cdot 10^5$) — the dimensions of Gregor's ceiling, and the maximum number of paint layers in a badly painted cell.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2\cdot 10^5$), the number of paint layers Amin applies to each row.</p><p>The third line contains $m$ integers $b_1, b_2, \ldots, b_m$ ($1 \le b_j \le 2\cdot 10^5$), the number of paint layers Benj applies to each column.</p></div><div class="output-specification"><p>Print a single integer, the number of badly painted regions.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $x$ ($1 \le n,m \le 2\cdot 10^5$, $1 \le x \le 2\cdot 10^5$) — the dimensions of Gregor's ceiling, and the maximum number of paint layers in a badly painted cell.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 2\cdot 10^5$), the number of paint layers Amin applies to each row.</p><p>The third line contains $m$ integers $b_1, b_2, \ldots, b_m$ ($1 \le b_j \le 2\cdot 10^5$), the number of paint layers Benj applies to each column.</p>

## Output

<p>Print a single integer, the number of badly painted regions.</p>





```input1
3 4 11
9 8 5
10 6 7 2
```




```input2
3 4 12
9 8 5
10 6 7 2
```




```input3
3 3 2
1 2 1
1 2 1
```




```input4
5 23 6
1 4 3 5 2
2 3 1 6 1 5 5 6 1 3 2 6 2 3 1 6 1 4 1 6 1 5 5
```




```output1
2
```




```output2
1
```




```output3
4
```




```output4
6
```



## Note

<p>The diagram below represents the first example. The numbers to the left of each row represent the list $a$, and the numbers above each column represent the list $b$. The numbers inside each cell represent the number of paint layers in that cell.</p><p>The colored cells correspond to badly painted cells. The red and blue cells respectively form $2$ badly painted regions.</p><center> <img class="tex-graphics" height="227px" src="file://Odbx0aHX.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center>
