## Description

<div><p>There is a grid with $n$ rows and $m$ columns. Every cell of the grid should be colored either blue or yellow.</p><p>A coloring of the grid is called stupid if every row has exactly one segment of blue cells and every column has exactly one segment of yellow cells.</p><p>In other words, every row must have at least one blue cell, and all blue cells in a row must be consecutive. Similarly, every column must have at least one yellow cell, and all yellow cells in a column must be consecutive.</p><center> <img class="tex-graphics" src="file://1uaeD7Lf.png" style="max-width: 100.0%;max-height: 100.0%;"> An example of a stupid coloring. </center><center> <img class="tex-graphics" src="file://YwqCYNJo.png" style="max-width: 100.0%;max-height: 100.0%;"> Examples of clever colorings. The first coloring is missing a blue cell in the second row, and the second coloring has two yellow segments in the second column. </center><p>How many stupid colorings of the grid are there? Two colorings are considered different if there is some cell that is colored differently.</p></div><div class="input-specification"><p>The only line contains two integers $n$, $m$ ($1\le n, m\le 2021$).</p></div><div class="output-specification"><p>Output a single integer — the number of stupid colorings modulo $998244353$.</p></div>

## Input

<p>The only line contains two integers $n$, $m$ ($1\le n, m\le 2021$).</p>

## Output

<p>Output a single integer — the number of stupid colorings modulo $998244353$.</p>





```input1
2 2
```




```input2
4 3
```




```input3
2020 2021
```




```output1
2
```




```output2
294
```




```output3
50657649
```



## Note

<p>In the first test case, these are the only two stupid $2\times 2$ colorings.</p><center> <img class="tex-graphics" src="file://JWfLQBXv.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
