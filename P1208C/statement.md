## Description

<div><p>Let us define a <span class="tex-font-style-it">magic</span> grid to be a square matrix of integers of size $n \times n$, satisfying the following conditions. </p><ul> <li> All integers from $0$ to $(n^2 - 1)$ inclusive appear in the matrix <span class="tex-font-style-bf">exactly once</span>. </li><li> <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">Bitwise XOR</a> of all elements in a row or a column must be the same for each row and column. </li></ul><p>You are given an integer $n$ which is a <span class="tex-font-style-bf">multiple of $4$</span>. Construct a <span class="tex-font-style-it">magic</span> grid of size $n \times n$.</p></div><div class="input-specification"><p>The only line of input contains an integer $n$ ($4 \leq n \leq 1000$). It is guaranteed that $n$ is a multiple of $4$.</p></div><div class="output-specification"><p>Print a <span class="tex-font-style-it">magic</span> grid, i.e. $n$ lines, the $i$-th of which contains $n$ space-separated integers, representing the $i$-th row of the grid.</p><p>If there are multiple answers, print any. We can show that an answer always exists.</p></div>

## Input

<p>The only line of input contains an integer $n$ ($4 \leq n \leq 1000$). It is guaranteed that $n$ is a multiple of $4$.</p>

## Output

<p>Print a <span class="tex-font-style-it">magic</span> grid, i.e. $n$ lines, the $i$-th of which contains $n$ space-separated integers, representing the $i$-th row of the grid.</p><p>If there are multiple answers, print any. We can show that an answer always exists.</p>





```input1
4
```




```input2
8
```




```output1
8 9 1 13
3 12 7 5
0 2 4 11
6 10 15 14
```




```output2
19 55 11 39 32 36 4 52
51 7 35 31 12 48 28 20
43 23 59 15 0 8 16 44
3 47 27 63 24 40 60 56
34 38 6 54 17 53 9 37
14 50 30 22 49 5 33 29
2 10 18 46 41 21 57 13
26 42 62 58 1 45 25 61
```



## Note

<p>In the first example, XOR of each row and each column is $13$.</p><p>In the second example, XOR of each row and each column is $60$.</p>
