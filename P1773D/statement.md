## Description

<div><p>Dora likes to play with dominoes. She takes $n \times m$ table, marks some cells as occupied, and then tries to fill all unoccupied cells with $2 \times 1$ dominoes.</p><center> <img class="tex-graphics" src="file://AkDbIUZr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Her little brother Dani loves to play pranks on his older sister. So when she is away, he marks two more unoccupied cells as occupied. He wants to do it in such a way that it will be impossible to fill all unoccupied cells with dominoes.</p><p>Help Dani to count the number of ways he can select these two cells. Since Dani can only count to one million, if this number of ways is $x$, output $\min(x, 10^6)$.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($1\le n, m\le 1000$). Next $n$ lines contain $m$ characters each&nbsp;— the initial state of the table. Character "<span class="tex-font-style-tt">#</span>" corresponds to an occupied cell, and character "<span class="tex-font-style-tt">.</span>" corresponds to an unoccupied cell. It is guaranteed that there are at least two unoccupied cells, and that it is possible to fill all unoccupied cells with dominoes.</p></div><div class="output-specification"><p>Let $x$ be the number of ways Dani can mark two cells in such a way that it will be impossible to fill all unoccupied cells with dominoes. </p><p>Print one integer $\min(x, 10^6)$.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($1\le n, m\le 1000$). Next $n$ lines contain $m$ characters each&nbsp;— the initial state of the table. Character "<span class="tex-font-style-tt">#</span>" corresponds to an occupied cell, and character "<span class="tex-font-style-tt">.</span>" corresponds to an unoccupied cell. It is guaranteed that there are at least two unoccupied cells, and that it is possible to fill all unoccupied cells with dominoes.</p>

## Output

<p>Let $x$ be the number of ways Dani can mark two cells in such a way that it will be impossible to fill all unoccupied cells with dominoes. </p><p>Print one integer $\min(x, 10^6)$.</p>





```input1
3 6
...#..
......
#...##
```




```input2
2 2
..
..
```




```input3
2 2
#.
#.
```




```output1
52
```




```output2
2
```




```output3
0
```


