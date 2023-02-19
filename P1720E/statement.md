## Description

<div><p>Misha has a <span class="tex-font-style-bf">square</span> $n \times n$ matrix, where the number in row $i$ and column $j$ is equal to $a_{i, j}$. Misha wants to modify the matrix to contain <span class="tex-font-style-bf">exactly</span> $k$ distinct integers. To achieve this goal, Misha can perform the following operation zero or more times:</p><ol> <li> choose any <span class="tex-font-style-bf">square</span> submatrix of the matrix (you choose $(x_1,y_1)$, $(x_2,y_2)$, such that $x_1 \leq x_2$, $y_1 \leq y_2$, $x_2 - x_1 = y_2 - y_1$, then submatrix is a set of cells with coordinates $(x, y)$, such that $x_1 \leq x \leq x_2$, $y_1 \leq y \leq y_2$), </li><li> choose an integer $k$, where $1 \leq k \leq n^2$, </li><li> replace all integers in the submatrix with $k$. </li></ol><p>Please find the minimum number of operations that Misha needs to achieve his goal.</p></div><div class="input-specification"><p>The first input line contains two integers $n$ and $k$ ($1 \leq n \leq 500, 1 \leq k \leq n^2$) &nbsp;— the size of the matrix and the desired amount of distinct elements in the matrix.</p><p>Then $n$ lines follows. The $i$-th of them contains $n$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, n}$ ($1 \leq a_{i,j} \leq n^2$) — the elements of the $i$-th row of the matrix.</p></div><div class="output-specification"><p>Output one integer — the minimum number of operations required.</p></div>

## Input

<p>The first input line contains two integers $n$ and $k$ ($1 \leq n \leq 500, 1 \leq k \leq n^2$) &nbsp;— the size of the matrix and the desired amount of distinct elements in the matrix.</p><p>Then $n$ lines follows. The $i$-th of them contains $n$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, n}$ ($1 \leq a_{i,j} \leq n^2$) — the elements of the $i$-th row of the matrix.</p>

## Output

<p>Output one integer — the minimum number of operations required.</p>





```input1
3 4
1 1 1
1 1 2
3 4 5
```




```input2
3 2
2 1 3
2 1 1
3 1 2
```




```input3
3 3
1 1 1
1 1 2
2 2 2
```




```input4
3 2
1 1 1
1 2 1
2 2 2
```




```output1
1
```




```output2
2
```




```output3
1
```




```output4
0
```



## Note

<p>In the first test case the answer is $1$, because one can change the value in the bottom right corner of the matrix to $1$. The resulting matrix can be found below:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-top">1</td><td class="tex-tabular-text-align-center tex-tabular-border-top">1</td><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top">1</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center">1</td><td class="tex-tabular-text-align-center">1</td><td class="tex-tabular-text-align-center tex-tabular-border-right">2</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-bottom">3</td><td class="tex-tabular-text-align-center tex-tabular-border-bottom">4</td><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">1</td></tr></tbody></table> </center><p>In the second test case the answer is $2$. First, one can change the entire matrix to contain only $1$s, and the change the value of any single cell to $2$. One of the possible resulting matrices is displayed below:</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-top">1</td><td class="tex-tabular-text-align-center tex-tabular-border-top">1</td><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top">1</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center">1</td><td class="tex-tabular-text-align-center">1</td><td class="tex-tabular-text-align-center tex-tabular-border-right">1</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-bottom">1</td><td class="tex-tabular-text-align-center tex-tabular-border-bottom">1</td><td class="tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-bottom">2</td></tr></tbody></table> </center>
