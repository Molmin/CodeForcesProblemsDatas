## Description

<div><p>You are given a tree consisting of $n$ vertices. A number is written on each vertex; the number on vertex $i$ is equal to $a_i$.</p><p>Let's denote the function $g(x, y)$ as the greatest common divisor of the numbers written on the vertices belonging to the simple path from vertex $x$ to vertex $y$ (including these two vertices).</p><p>For every integer from $1$ to $2 \cdot 10^5$ you have to count the number of pairs $(x, y)$ $(1 \le x \le y \le n)$ such that $g(x, y)$ is equal to this number.</p></div><div class="input-specification"><p>The first line contains one integer $n$ — the number of vertices $(1 \le n \le 2 \cdot 10^5)$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ $(1 \le a_i \le 2 \cdot 10^5)$ — the numbers written on vertices.</p><p>Then $n - 1$ lines follow, each containing two integers $x$ and $y$ $(1 \le x, y \le n, x \ne y)$ denoting an edge connecting vertex $x$ with vertex $y$. It is guaranteed that these edges form a tree.</p></div><div class="output-specification"><p>For every integer $i$ from $1$ to $2 \cdot 10^5$ do the following: if there is no pair $(x, y)$ such that $x \le y$ and $g(x, y) = i$, don't output anything. Otherwise output two integers: $i$ and the number of aforementioned pairs. You have to consider the values of $i$ in ascending order.</p><p>See the examples for better understanding.</p></div>

## Input

<p>The first line contains one integer $n$ — the number of vertices $(1 \le n \le 2 \cdot 10^5)$.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ $(1 \le a_i \le 2 \cdot 10^5)$ — the numbers written on vertices.</p><p>Then $n - 1$ lines follow, each containing two integers $x$ and $y$ $(1 \le x, y \le n, x \ne y)$ denoting an edge connecting vertex $x$ with vertex $y$. It is guaranteed that these edges form a tree.</p>

## Output

<p>For every integer $i$ from $1$ to $2 \cdot 10^5$ do the following: if there is no pair $(x, y)$ such that $x \le y$ and $g(x, y) = i$, don't output anything. Otherwise output two integers: $i$ and the number of aforementioned pairs. You have to consider the values of $i$ in ascending order.</p><p>See the examples for better understanding.</p>





```input1
3
1 2 3
1 2
2 3

```




```input2
6
1 2 4 8 16 32
1 6
6 3
3 4
4 2
6 5

```




```input3
4
9 16 144 6
1 3
2 3
4 3

```




```output1
1 4
2 1
3 1

```




```output2
1 6
2 5
4 6
8 1
16 2
32 1

```




```output3
1 1
2 1
3 1
6 2
9 2
16 2
144 1

```


