## Description

<div><p>Petya collects <span class="tex-font-style-it">beautiful</span> matrix.</p><p>A matrix of size $n \times n$ is <span class="tex-font-style-it">beautiful</span> if: </p><ul> <li> All elements of the matrix are integers between $1$ and $n$; </li><li> For every row of the matrix, all elements of this row are different; </li><li> For every pair of vertically adjacent elements, these elements are different. </li></ul><p>Today Petya bought a <span class="tex-font-style-it">beautiful</span> matrix $a$ of size $n \times n$, and now he wants to determine its rarity.</p><p>The rarity of the matrix is its index in the list of <span class="tex-font-style-it">beautiful</span> matrices of size $n \times n$, sorted in lexicographical order. Matrix comparison is done row by row. (The index of lexicographically smallest matrix is <span class="tex-font-style-bf">zero</span>).</p><p>Since the number of <span class="tex-font-style-it">beautiful</span> matrices may be huge, Petya wants you to calculate the rarity of the matrix $a$ modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2000$) — the number of rows and columns in $a$.</p><p>Each of the next $n$ lines contains $n$ integers $a_{i,j}$ ($1 \le a_{i,j} \le n$) — the elements of $a$.</p><p>It is guaranteed that $a$ is a <span class="tex-font-style-it">beautiful</span> matrix.</p></div><div class="output-specification"><p>Print one integer — the rarity of matrix $a$, taken modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2000$) — the number of rows and columns in $a$.</p><p>Each of the next $n$ lines contains $n$ integers $a_{i,j}$ ($1 \le a_{i,j} \le n$) — the elements of $a$.</p><p>It is guaranteed that $a$ is a <span class="tex-font-style-it">beautiful</span> matrix.</p>

## Output

<p>Print one integer — the rarity of matrix $a$, taken modulo $998\,244\,353$.</p>





```input1
2
2 1
1 2
```




```input2
3
1 2 3
2 3 1
3 1 2
```




```input3
3
1 2 3
3 1 2
2 3 1
```




```output1
1
```




```output2
1
```




```output3
3
```



## Note

<p>There are only $2$ <span class="tex-font-style-it">beautiful</span> matrices of size $2 \times 2$:</p><center> <img class="tex-graphics" src="file://KqbhV0fj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are the first $5$ <span class="tex-font-style-it">beautiful</span> matrices of size $3 \times 3$ in lexicographical order:</p><center> <img class="tex-graphics" src="file://sjVVSpSG.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
