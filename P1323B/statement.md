## Description

<div><p>You are given an array $a$ of length $n$ and array $b$ of length $m$ both consisting of only integers $0$ and $1$. Consider a matrix $c$ of size $n \times m$ formed by following rule: $c_{i, j} = a_i \cdot b_j$ (i.e. $a_i$ multiplied by $b_j$). It's easy to see that $c$ consists of only zeroes and ones too.</p><p>How many <span class="tex-font-style-it">subrectangles</span> of size (area) $k$ consisting only of ones are there in $c$?</p><p>A <span class="tex-font-style-it">subrectangle</span> is an intersection of a consecutive (subsequent) segment of rows and a consecutive (subsequent) segment of columns. I.e. consider four integers $x_1, x_2, y_1, y_2$ ($1 \le x_1 \le x_2 \le n$, $1 \le y_1 \le y_2 \le m$) a subrectangle $c[x_1 \dots x_2][y_1 \dots y_2]$ is an intersection of the rows $x_1, x_1+1, x_1+2, \dots, x_2$ and the columns $y_1, y_1+1, y_1+2, \dots, y_2$.</p><p>The size (area) of a subrectangle is the total number of cells in it.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($1 \leq n, m \leq 40\,000, 1 \leq k \leq n \cdot m$), length of array $a$, length of array $b$ and required size of subrectangles.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 1$), elements of $a$.</p><p>The third line contains $m$ integers $b_1, b_2, \ldots, b_m$ ($0 \leq b_i \leq 1$), elements of $b$.</p></div><div class="output-specification"><p>Output single integer&nbsp;— the number of subrectangles of $c$ with size (area) $k$ consisting only of ones.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($1 \leq n, m \leq 40\,000, 1 \leq k \leq n \cdot m$), length of array $a$, length of array $b$ and required size of subrectangles.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 1$), elements of $a$.</p><p>The third line contains $m$ integers $b_1, b_2, \ldots, b_m$ ($0 \leq b_i \leq 1$), elements of $b$.</p>

## Output

<p>Output single integer&nbsp;— the number of subrectangles of $c$ with size (area) $k$ consisting only of ones.</p>





```input1
3 3 2
1 0 1
1 1 1
```




```input2
3 5 4
1 1 1
1 1 1 1 1
```




```output1
4
```




```output2
14
```



## Note

<p>In first example matrix $c$ is:</p><center> <img class="tex-graphics" src="file://MgFp9RaL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are $4$ subrectangles of size $2$ consisting of only ones in it:</p><center> <img class="tex-graphics" src="file://B1nDXmNr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In second example matrix $c$ is:</p><center> <img class="tex-graphics" src="file://p1uxZoyt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
