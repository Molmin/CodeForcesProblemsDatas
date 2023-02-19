## Description

<div><p>Egor has a table of size $n \times m$, with lines numbered from $1$ to $n$ and columns numbered from $1$ to $m$. Each cell has a color that can be presented as an integer from $1$ to $10^5$.</p><p>Let us denote the cell that lies in the intersection of the $r$-th row and the $c$-th column as $(r, c)$. We define the <span class="tex-font-style-underline">manhattan distance</span> between two cells $(r_1, c_1)$ and $(r_2, c_2)$ as the length of a shortest path between them where each consecutive cells in the path must have a common side. The path can go through cells of any color. For example, in the table $3 \times 4$ the manhattan distance between $(1, 2)$ and $(3, 3)$ is $3$, one of the shortest paths is the following: $(1, 2) \to (2, 2) \to (2, 3) \to (3, 3)$. </p><p>Egor decided to calculate the sum of manhattan distances between each pair of cells of the same color. Help him to calculate this sum.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n \le m$, $n \cdot m \leq 100\,000$)&nbsp;— number of rows and columns in the table.</p><p>Each of next $n$ lines describes a row of the table. The $i$-th line contains $m$ integers $c_{i1}, c_{i2}, \ldots, c_{im}$ ($1 \le c_{ij} \le 100\,000$)&nbsp;— colors of cells in the $i$-th row.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the the sum of manhattan distances between each pair of cells of the same color.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n \le m$, $n \cdot m \leq 100\,000$)&nbsp;— number of rows and columns in the table.</p><p>Each of next $n$ lines describes a row of the table. The $i$-th line contains $m$ integers $c_{i1}, c_{i2}, \ldots, c_{im}$ ($1 \le c_{ij} \le 100\,000$)&nbsp;— colors of cells in the $i$-th row.</p>

## Output

<p>Print one integer&nbsp;— the the sum of manhattan distances between each pair of cells of the same color.</p>





```input1
2 3
1 2 3
3 2 1
```




```input2
3 4
1 1 2 2
2 1 1 2
2 2 1 1
```




```input3
4 4
1 1 2 3
2 1 1 2
3 1 2 1
1 1 2 1
```




```output1
7
```




```output2
76
```




```output3
129
```



## Note

<p>In the first sample there are three pairs of cells of same color: in cells $(1, 1)$ and $(2, 3)$, in cells $(1, 2)$ and $(2, 2)$, in cells $(1, 3)$ and $(2, 1)$. The manhattan distances between them are $3$, $1$ and $3$, the sum is $7$.</p>
