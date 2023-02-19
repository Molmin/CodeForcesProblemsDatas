## Description

<div><p>Burenka has two pictures $a$ and $b$, which are tables of the same size $n \times m$. Each cell of each painting has a color — a number from $0$ to $2 \cdot 10^5$, and there are no repeating colors in any row or column of each of the two paintings, except color $0$.</p><p>Burenka wants to get a picture $b$ from the picture $a$. To achieve her goal, Burenka can perform one of $2$ operations: swap any two rows of $a$ or any two of its columns. Tell Burenka if she can fulfill what she wants, and if so, tell her the sequence of actions.</p><p>The rows are numbered from $1$ to $n$ from top to bottom, the columns are numbered from $1$ to $m$ from left to right.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n \cdot m \leq 2 \cdot 10^5$) — the sizes of the table.</p><p>The $i$-th of the next $n$ lines contains $m$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, m}$ ($0 \leq a_{i,j} \leq 2 \cdot 10^5$)&nbsp;— the colors of the $i$-th row of picture $a$. It is guaranteed that there are no identical colors in the same row or column, except color $0$.</p><p>The $i$-th of the following $n$ lines contains $m$ integers $b_{i, 1}, b_{i, 2}, \ldots, b_{i, m}$ ($0 \leq b_{i,j} \leq 2 \cdot 10^5$)&nbsp;— the colors of the $i$-th row of picture $b$. It is guaranteed that there are no identical colors in the same row or column, except color $0$.</p></div><div class="output-specification"><p>In the first line print the number $-1$ if it is impossible to achieve what Burenka wants, otherwise print the number of actions in your solution $k$ ($0 \le k \le 2 \cdot 10^5$). It can be proved that if a solution exists, then there exists a solution where $k \le 2 \cdot 10^5$.</p><p>In the next $k$ lines print the operations. First print the type of the operation ($1$ — swap rows, $2$ — columns), and then print the two indices of rows or columns to which the operation is applied.</p><p>Note that you don't have to minimize the number of operations.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n \cdot m \leq 2 \cdot 10^5$) — the sizes of the table.</p><p>The $i$-th of the next $n$ lines contains $m$ integers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, m}$ ($0 \leq a_{i,j} \leq 2 \cdot 10^5$)&nbsp;— the colors of the $i$-th row of picture $a$. It is guaranteed that there are no identical colors in the same row or column, except color $0$.</p><p>The $i$-th of the following $n$ lines contains $m$ integers $b_{i, 1}, b_{i, 2}, \ldots, b_{i, m}$ ($0 \leq b_{i,j} \leq 2 \cdot 10^5$)&nbsp;— the colors of the $i$-th row of picture $b$. It is guaranteed that there are no identical colors in the same row or column, except color $0$.</p>

## Output

<p>In the first line print the number $-1$ if it is impossible to achieve what Burenka wants, otherwise print the number of actions in your solution $k$ ($0 \le k \le 2 \cdot 10^5$). It can be proved that if a solution exists, then there exists a solution where $k \le 2 \cdot 10^5$.</p><p>In the next $k$ lines print the operations. First print the type of the operation ($1$ — swap rows, $2$ — columns), and then print the two indices of rows or columns to which the operation is applied.</p><p>Note that you don't have to minimize the number of operations.</p>





```input1
3 3
1 0 2
0 0 0
2 0 1
2 0 1
0 0 0
1 0 2
```




```input2
4 4
0 0 1 2
3 0 0 0
0 1 0 0
1 0 0 0
2 0 0 1
0 3 0 0
0 1 0 0
0 0 1 0
```




```input3
3 3
1 2 0
0 0 0
0 0 0
1 0 0
2 0 0
0 0 0
```




```output1
1
1 1 3
```




```output2
4
1 3 4
2 3 4
2 2 3
2 1 2
```




```output3
-1
```


