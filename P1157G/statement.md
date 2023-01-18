## Description

<div><p>You are given a binary matrix $a$ of size $n \times m$. A binary matrix is a matrix where each element is either $0$ or $1$.</p><p>You may perform some (possibly zero) operations with this matrix. During each operation you can inverse the row of this matrix or a column of this matrix. Formally, inverting a row is changing all values in this row to the opposite ($0$ to $1$, $1$ to $0$). Inverting a column is changing all values in this column to the opposite.</p><p>Your task is to sort the initial matrix by some sequence of such operations. The matrix is considered <span class="tex-font-style-bf">sorted</span> if the array $[a_{1, 1}, a_{1, 2}, \dots, a_{1, m}, a_{2, 1}, a_{2, 2}, \dots, a_{2, m}, \dots, a_{n, m - 1}, a_{n, m}]$ is sorted <span class="tex-font-style-it">in non-descending order</span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 200$) — the number of rows and the number of columns in the matrix.</p><p>The next $n$ lines contain $m$ integers each. The $j$-th element in the $i$-th line is $a_{i, j}$ ($0 \le a_{i, j} \le 1$) — the element of $a$ at position $(i, j)$.</p></div><div class="output-specification"><p>If it is impossible to obtain a <span class="tex-font-style-bf">sorted</span> matrix, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line print a string $r$ of length $n$. The $i$-th character $r_i$ of this string should be '<span class="tex-font-style-tt">1</span>' if the $i$-th row of the matrix is inverted and '<span class="tex-font-style-tt">0</span>' otherwise. In the third line print a string $c$ of length $m$. The $j$-th character $c_j$ of this string should be '<span class="tex-font-style-tt">1</span>' if the $j$-th column of the matrix is inverted and '<span class="tex-font-style-tt">0</span>' otherwise. If there are multiple answers, you can print any.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 200$) — the number of rows and the number of columns in the matrix.</p><p>The next $n$ lines contain $m$ integers each. The $j$-th element in the $i$-th line is $a_{i, j}$ ($0 \le a_{i, j} \le 1$) — the element of $a$ at position $(i, j)$.</p>

## Output

<p>If it is impossible to obtain a <span class="tex-font-style-bf">sorted</span> matrix, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line print a string $r$ of length $n$. The $i$-th character $r_i$ of this string should be '<span class="tex-font-style-tt">1</span>' if the $i$-th row of the matrix is inverted and '<span class="tex-font-style-tt">0</span>' otherwise. In the third line print a string $c$ of length $m$. The $j$-th character $c_j$ of this string should be '<span class="tex-font-style-tt">1</span>' if the $j$-th column of the matrix is inverted and '<span class="tex-font-style-tt">0</span>' otherwise. If there are multiple answers, you can print any.</p>





```input1
2 2
1 1
0 1
```




```input2
3 4
0 0 0 1
0 0 0 0
1 1 1 1
```




```input3
3 3
0 0 0
1 0 1
1 1 0
```




```output1
YES
00
10
```




```output2
YES
010
0000
```




```output3
NO
```


