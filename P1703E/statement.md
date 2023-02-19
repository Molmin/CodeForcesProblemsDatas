## Description

<div><p>You are given a square grid with $n$ rows and $n$ columns. Each cell contains either $0$ or $1$. </p><p>In an operation, you can select a cell of the grid and flip it (from $0 \to 1$ or $1 \to 0$). Find the minimum number of operations you need to obtain a square that remains the same when rotated $0^{\circ}$, $90^{\circ}$, $180^{\circ}$ and $270^{\circ}$.</p><p>The picture below shows an example of all rotations of a grid.</p><center> <img class="tex-graphics" src="file://iX17Xjn7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the size of the grid.</p><p>Then $n$ lines follow, each with $n$ characters $a_{i,j}$ ($0 \leq a_{i,j} \leq 1$)&nbsp;— the number written in each cell.</p></div><div class="output-specification"><p>For each test case output a single integer &nbsp;— the minimum number of operations needed to make the square look the same rotated $0^{\circ}$, $90^{\circ}$, $180^{\circ}$ and $270^{\circ}$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the size of the grid.</p><p>Then $n$ lines follow, each with $n$ characters $a_{i,j}$ ($0 \leq a_{i,j} \leq 1$)&nbsp;— the number written in each cell.</p>

## Output

<p>For each test case output a single integer &nbsp;— the minimum number of operations needed to make the square look the same rotated $0^{\circ}$, $90^{\circ}$, $180^{\circ}$ and $270^{\circ}$.</p>





```input1|2,3,4,5,8,9,10,11,12,13,20,21,22,23,24,25
5
3
010
110
010
1
0
5
11100
11011
01011
10011
11000
5
01000
10101
01010
00010
01001
5
11001
00000
11111
10110
01111
```




```output1
1
0
9
7
6
```



## Note

<p>In the first test case, we can perform one operations to make the grid $\begin{matrix}0 &amp; 1 &amp; 0\\ 1 &amp; 1 &amp; \color{red}{1}\\ 0 &amp; 1 &amp; 0\end{matrix}$. Now, all rotations of the square are the same.</p><p>In the second test case, all rotations of the square are already the same, so we don't need any flips.</p>
