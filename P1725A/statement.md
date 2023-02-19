## Description

<div><p>Pak Chanek has a grid that has $N$ rows and $M$ columns. Each row is numbered from $1$ to $N$ from top to bottom. Each column is numbered from $1$ to $M$ from left to right.</p><p>Each tile in the grid contains a number. The numbers are arranged as follows: </p><ul> <li> Row $1$ contains integers from $1$ to $M$ from left to right. </li><li> Row $2$ contains integers from $M+1$ to $2 \times M$ from left to right. </li><li> Row $3$ contains integers from $2 \times M+1$ to $3 \times M$ from left to right. </li><li> And so on until row $N$. </li></ul><p>A domino is defined as two different tiles in the grid that touch <span class="tex-font-style-bf">by their sides</span>. A domino is said to be <span class="tex-font-style-bf">tight</span> if and only if the two numbers in the domino have a difference of exactly $1$. Count the number of distinct <span class="tex-font-style-bf">tight</span> dominoes in the grid.</p><p>Two dominoes are said to be distinct if and only if there exists at least one tile that is in one domino, but not in the other.</p></div><div class="input-specification"><p>The only line contains two integers $N$ and $M$ ($1 \leq N, M \leq 10^9$) — the number of rows and columns in the grid.</p></div><div class="output-specification"><p>An integer representing the number of distinct <span class="tex-font-style-bf">tight</span> dominoes in the grid.</p></div>

## Input

<p>The only line contains two integers $N$ and $M$ ($1 \leq N, M \leq 10^9$) — the number of rows and columns in the grid.</p>

## Output

<p>An integer representing the number of distinct <span class="tex-font-style-bf">tight</span> dominoes in the grid.</p>





```input1
3 4
```




```input2
2 1
```




```output1
9
```




```output2
1
```



## Note

<p>The picture below is the grid that Pak Chanek has in the first example.</p><center> <img class="tex-graphics" src="file://CmLU3RhG.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>The picture below is an example of a <span class="tex-font-style-bf">tight</span> domino in the grid.</p><center> <img class="tex-graphics" src="file://lPSqTPw7.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center>
