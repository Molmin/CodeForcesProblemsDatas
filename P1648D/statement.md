## Description

<div><p>Dima is taking part in a show organized by his friend Peter. In this show Dima is required to cross a $3 \times n$ rectangular field. Rows are numbered from $1$ to $3$ and columns are numbered from $1$ to $n$.</p><p>The cell in the intersection of the $i$-th row and the $j$-th column of the field contains an integer $a_{i,j}$. Initially Dima's score equals zero, and whenever Dima reaches a cell in the row $i$ and the column $j$, his score changes by $a_{i,j}$. Note that the score can become negative.</p><p>Initially all cells in the first and the third row are marked as available, and all cells in the second row are marked as unavailable. However, Peter offered Dima some help: there are $q$ special offers in the show, the $i$-th special offer allows Dima to mark cells in the second row between $l_i$ and $r_i$ as available, though Dima's score reduces by $k_i$ whenever he accepts a special offer. Dima is allowed to use as many special offers as he wants, and might mark the same cell as available multiple times.</p><p>Dima starts his journey in the cell $(1, 1)$ and would like to reach the cell $(3, n)$. He can move either down to the next row or right to the next column (meaning he could increase the current row or column by 1), thus making $n + 1$ moves in total, out of which exactly $n - 1$ would be horizontal and $2$ would be vertical.</p><p>Peter promised Dima to pay him based on his final score, so the sum of all numbers of all visited cells minus the cost of all special offers used. Please help Dima to maximize his final score.</p></div><div class="input-specification"><p>The first input line contains two integers $n$ and $q$ ($1 \le n, q \le 500\,000$)&nbsp;— the number of columns in the field and the number of special offers.</p><p>The next three lines describe the field, $i$-th of them contains $n$ integers $a_{i1}$, $a_{i2}$, ..., $a_{in}$ ($-10^9 \le a_{ij} \le 10^9)$&nbsp;— the values in the $i$-th row.</p><p>The next $q$ lines describe special offers: the $i$-th offer is described by 3 integers $l_i$, $r_i$ and $k_i$ ($1 \leq l_i \leq r_i \leq n$, $1\leq k_i\leq 10^9$)&nbsp;— the segment that becomes unblocked and the cost of this special offer.</p></div><div class="output-specification"><p>Output one integer&nbsp;— the maximum final score Dima can achieve.</p></div>

## Input

<p>The first input line contains two integers $n$ and $q$ ($1 \le n, q \le 500\,000$)&nbsp;— the number of columns in the field and the number of special offers.</p><p>The next three lines describe the field, $i$-th of them contains $n$ integers $a_{i1}$, $a_{i2}$, ..., $a_{in}$ ($-10^9 \le a_{ij} \le 10^9)$&nbsp;— the values in the $i$-th row.</p><p>The next $q$ lines describe special offers: the $i$-th offer is described by 3 integers $l_i$, $r_i$ and $k_i$ ($1 \leq l_i \leq r_i \leq n$, $1\leq k_i\leq 10^9$)&nbsp;— the segment that becomes unblocked and the cost of this special offer.</p>

## Output

<p>Output one integer&nbsp;— the maximum final score Dima can achieve.</p>





```input1
4 3
1 0 2 -1
-3 1 9 2
3 2 4 1
1 2 5
2 3 4
1 4 14
```




```input2
5 4
-20 -10 -11 -10 1
1 3 3 6 3
14 -20 3 6 2
1 5 13
1 2 2
3 5 3
2 3 1
```




```output1
13
```




```output2
-4
```



## Note

<p>In the first example, it is optimal to use Peter's second offer of $4$ rubles and go through the cells $(1, 1)$, $(1, 2)$, $(1, 3)$, $(2, 3)$, $(3, 3)$, $(3, 4)$, earning $1 + 0 + 2 + 9 + 4 + 1 - 4 = 13$ rubles in total.</p><p>In the second example, it is optimal to use Peter's second and third offers of $2$ and $3$ rubles, respectively, and go through the cells $(1, 1)$, $(2, 1)$, $(2, 2)$, $(2, 3)$, $(2, 4)$, $(3, 4)$, $(3, 5)$, earning $-20 + 1 + 3 + 3 + 6 + 6 + 2 - 2 - 3= -4$ rubles.</p>
