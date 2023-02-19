## Description

<div><p>Circular land is an $2n \times 2n$ grid. Rows of this grid are numbered by integers from $1$ to $2n$ from top to bottom and columns of this grid are numbered by integers from $1$ to $2n$ from left to right. The cell $(x, y)$ is the cell on the intersection of row $x$ and column $y$ for $1 \leq x \leq 2n$ and $1 \leq y \leq 2n$.</p><p>There are $n^2$ of your friends in the top left corner of the grid. That is, in each cell $(x, y)$ with $1 \leq x, y \leq n$ there is exactly one friend. Some of the other cells are covered with snow.</p><p>Your friends want to get to the bottom right corner of the grid. For this in each cell $(x, y)$ with $n+1 \leq x, y \leq 2n$ there should be exactly one friend. It doesn't matter in what cell each of friends will be.</p><p>You have decided to help your friends to get to the bottom right corner of the grid.</p><p>For this, you can give instructions of the following types: </p><ul> <li> You select a row $x$. All friends in this row should move to the next cell in this row. That is, friend from the cell $(x, y)$ with $1 \leq y &lt; 2n$ will move to the cell $(x, y + 1)$ and friend from the cell $(x, 2n)$ will move to the cell $(x, 1)$. </li><li> You select a row $x$. All friends in this row should move to the previous cell in this row. That is, friend from the cell $(x, y)$ with $1 &lt; y \leq 2n$ will move to the cell $(x, y - 1)$ and friend from the cell $(x, 1)$ will move to the cell $(x, 2n)$. </li><li> You select a column $y$. All friends in this column should move to the next cell in this column. That is, friend from the cell $(x, y)$ with $1 \leq x &lt; 2n$ will move to the cell $(x + 1, y)$ and friend from the cell $(2n, y)$ will move to the cell $(1, y)$. </li><li> You select a column $y$. All friends in this column should move to the previous cell in this column. That is, friend from the cell $(x, y)$ with $1 &lt; x \leq 2n$ will move to the cell $(x - 1, y)$ and friend from the cell $(1, y)$ will move to the cell $(2n, y)$. </li></ul><p>Note how friends on the grid border behave in these instructions.</p><center> <img class="tex-graphics" src="file://w2SQbaWq.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">Example of applying the third operation to the second column. Here, colorful circles denote your friends and blue cells are covered with snow.</span> </center><p>You can give such instructions any number of times. You can give instructions of different types. If after any instruction one of your friends is in the cell covered with snow he becomes ill.</p><p>In order to save your friends you can remove snow from some cells before giving the first instruction: </p><ul> <li> You can select the cell $(x, y)$ that is covered with snow now and remove snow from this cell for $c_{x, y}$ coins. </li></ul><p>You can do this operation any number of times.</p><p>You want to spend the minimal number of coins and give some instructions to your friends. After this, all your friends should be in the bottom right corner of the grid and none of them should be ill.</p><p>Please, find how many coins you will spend.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($1 \leq n \leq 250$).</p><p>Each of the next $2n$ lines contains $2n$ integers $c_{i, 1}, c_{i, 2}, \ldots, c_{i, 2n}$ ($0 \leq c_{i, j} \leq 10^9$)&nbsp;— costs of removing snow from cells. If $c_{i, j} = 0$ for some $i, j$ than there is no snow in cell $(i, j)$. Otherwise, cell $(i, j)$ is covered with snow.</p><p>It is guaranteed that $c_{i, j} = 0$ for $1 \leq i, j \leq n$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $250$.</p></div><div class="output-specification"><p>For each test case output one integer&nbsp;— the minimal number of coins you should spend.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($1 \leq n \leq 250$).</p><p>Each of the next $2n$ lines contains $2n$ integers $c_{i, 1}, c_{i, 2}, \ldots, c_{i, 2n}$ ($0 \leq c_{i, j} \leq 10^9$)&nbsp;— costs of removing snow from cells. If $c_{i, j} = 0$ for some $i, j$ than there is no snow in cell $(i, j)$. Otherwise, cell $(i, j)$ is covered with snow.</p><p>It is guaranteed that $c_{i, j} = 0$ for $1 \leq i, j \leq n$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $250$.</p>

## Output

<p>For each test case output one integer&nbsp;— the minimal number of coins you should spend.</p>





```input1
4
1
0 8
1 99
2
0 0 0 0
0 0 0 0
9 9 2 2
9 9 9 9
2
0 0 4 2
0 0 2 4
4 2 4 2
2 4 2 4
4
0 0 0 0 0 0 0 2
0 0 0 0 0 0 2 0
0 0 0 0 0 2 0 0
0 0 0 0 2 0 0 0
0 0 0 2 2 0 2 2
0 0 2 0 1 6 2 1
0 2 0 0 2 4 7 4
2 0 0 0 2 0 1 6
```




```output1
100
22
14
42
```



## Note

<p>In the first test case you can remove snow from the cells $(2, 1)$ and $(2, 2)$ for $100$ coins. Then you can give instructions </p><ul> <li> All friends in the first collum should move to the previous cell. After this, your friend will be in the cell $(2, 1)$. </li><li> All friends in the second row should move to the next cell. After this, your friend will be in the cell $(2, 2)$. </li></ul><p>In the second test case you can remove all snow from the columns $3$ and $4$ for $22$ coins. Then you can give instructions </p><ul> <li> All friends in the first row should move to the next cell. </li><li> All friends in the first row should move to the next cell. </li><li> All friends in the second row should move to the next cell. </li><li> All friends in the second row should move to the next cell. </li><li> All friends in the third column should move to the next cell. </li><li> All friends in the third column should move to the next cell. </li><li> All friends in the fourth column should move to the next cell. </li><li> All friends in the fourth column should move to the next cell. </li></ul><p>It can be shown that none of the friends will become ill and that it is impossible to spend less coins.</p>
