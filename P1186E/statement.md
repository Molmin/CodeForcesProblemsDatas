## Description

<div><p>Vus the Cossack has a field with dimensions $n \times m$, which consists of "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>". He is building an infinite field from this field. He is doing this in this way:</p><ol><li> He takes the current field and finds a new inverted field. In other words, the new field will contain "<span class="tex-font-style-tt">1</span>" only there, where "<span class="tex-font-style-tt">0</span>" was in the current field, and "<span class="tex-font-style-tt">0</span>" there, where "<span class="tex-font-style-tt">1</span>" was.</li><li> To the current field, he adds the inverted field to the right. </li><li> To the current field, he adds the inverted field to the bottom. </li><li> To the current field, he adds the current field to the bottom right. </li><li> He repeats it.</li></ol><p>For example, if the initial field was:</p><center> $\begin{matrix} 1 &amp; 0 &amp; \\ 1 &amp; 1 &amp; \\ \end{matrix}$ </center><p>After the first iteration, the field will be like this:</p><center> $\begin{matrix} 1 &amp; 0 &amp; 0 &amp; 1 \\ 1 &amp; 1 &amp; 0 &amp; 0 \\ 0 &amp; 1 &amp; 1 &amp; 0 \\ 0 &amp; 0 &amp; 1 &amp; 1 \\ \end{matrix}$ </center><p>After the second iteration, the field will be like this:</p><center> $\begin{matrix} 1 &amp; 0 &amp; 0 &amp; 1 &amp; 0 &amp; 1 &amp; 1 &amp; 0 \\ 1 &amp; 1 &amp; 0 &amp; 0 &amp; 0 &amp; 0 &amp; 1 &amp; 1 \\ 0 &amp; 1 &amp; 1 &amp; 0 &amp; 1 &amp; 0 &amp; 0 &amp; 1 \\ 0 &amp; 0 &amp; 1 &amp; 1 &amp; 1 &amp; 1 &amp; 0 &amp; 0 \\ 0 &amp; 1 &amp; 1 &amp; 0 &amp; 1 &amp; 0 &amp; 0 &amp; 1 \\ 0 &amp; 0 &amp; 1 &amp; 1 &amp; 1 &amp; 1 &amp; 0 &amp; 0 \\ 1 &amp; 0 &amp; 0 &amp; 1 &amp; 0 &amp; 1 &amp; 1 &amp; 0 \\ 1 &amp; 1 &amp; 0&amp; 0 &amp; 0 &amp; 0 &amp; 1 &amp; 1 \\ \end{matrix}$ </center><p>And so on...</p><p>Let's numerate lines from top to bottom from $1$ to infinity, and columns from left to right from $1$ to infinity. We call the submatrix $(x_1, y_1, x_2, y_2)$ all numbers that have coordinates $(x, y)$ such that $x_1 \leq x \leq x_2$ and $y_1 \leq y \leq y_2$.</p><p>The Cossack needs sometimes to find the sum of all the numbers in submatrices. Since he is pretty busy right now, he is asking you to find the answers!</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, $q$ ($1 \leq n, m \leq 1\,000$, $1 \leq q \leq 10^5$)&nbsp;— the dimensions of the initial matrix and the number of queries.</p><p>Each of the next $n$ lines contains $m$ characters $c_{ij}$ ($0 \leq c_{ij} \leq 1$)&nbsp;— the characters in the matrix.</p><p>Each of the next $q$ lines contains four integers $x_1$, $y_1$, $x_2$, $y_2$ ($1 \leq x_1 \leq x_2 \leq 10^9$, $1 \leq y_1 \leq y_2 \leq 10^9$)&nbsp;— the coordinates of the upper left cell and bottom right cell, between which you need to find the sum of all numbers.</p></div><div class="output-specification"><p>For each query, print the answer.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, $q$ ($1 \leq n, m \leq 1\,000$, $1 \leq q \leq 10^5$)&nbsp;— the dimensions of the initial matrix and the number of queries.</p><p>Each of the next $n$ lines contains $m$ characters $c_{ij}$ ($0 \leq c_{ij} \leq 1$)&nbsp;— the characters in the matrix.</p><p>Each of the next $q$ lines contains four integers $x_1$, $y_1$, $x_2$, $y_2$ ($1 \leq x_1 \leq x_2 \leq 10^9$, $1 \leq y_1 \leq y_2 \leq 10^9$)&nbsp;— the coordinates of the upper left cell and bottom right cell, between which you need to find the sum of all numbers.</p>

## Output

<p>For each query, print the answer.</p>





```input1
2 2 5
10
11
1 1 8 8
2 4 5 6
1 2 7 8
3 3 6 8
5 6 7 8
```




```input2
2 3 7
100
101
4 12 5 17
5 4 9 4
1 4 13 18
12 1 14 9
3 10 7 18
3 15 12 17
8 6 8 12
```




```output1
32
5
25
14
4
```




```output2
6
3
98
13
22
15
3
```



## Note

<p>The first example is explained in the legend.</p>
