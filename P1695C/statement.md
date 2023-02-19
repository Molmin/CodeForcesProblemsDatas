## Description

<div><p>You are given a grid with $n$ rows and $m$ columns. We denote the square on the $i$-th ($1\le i\le n$) row and $j$-th ($1\le j\le m$) column by $(i, j)$ and the number there by $a_{ij}$. All numbers are equal to $1$ or to $-1$. </p><p>You start from the square $(1, 1)$ and can move one square down or one square to the right at a time. In the end, you want to end up at the square $(n, m)$.</p><p>Is it possible to move in such a way so that the sum of the values written in all the visited cells (including $a_{11}$ and $a_{nm}$) is $0$?</p><center><img class="tex-graphics" src="file://ibGEsurp.png" style="max-width: 100.0%;max-height: 100.0%;"></center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 1000$) &nbsp;— the size of the grid.</p><p>Each of the following $n$ lines contains $m$ integers. The $j$-th integer on the $i$-th line is $a_{ij}$ ($a_{ij} = 1$ or $-1$) &nbsp;— the element in the cell $(i, j)$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, print "YES" if there exists a path from the top left to the bottom right that adds up to $0$, and "NO" otherwise. You can output each letter in any case.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 1000$) &nbsp;— the size of the grid.</p><p>Each of the following $n$ lines contains $m$ integers. The $j$-th integer on the $i$-th line is $a_{ij}$ ($a_{ij} = 1$ or $-1$) &nbsp;— the element in the cell $(i, j)$.</p><p>It is guaranteed that the sum of $n\cdot m$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, print "YES" if there exists a path from the top left to the bottom right that adds up to $0$, and "NO" otherwise. You can output each letter in any case.</p>





```input1|2,3,6,7,12,13,14,15
5
1 1
1
1 2
1 -1
1 4
1 -1 1 -1
3 4
1 -1 -1 -1
-1 1 1 -1
1 1 1 -1
3 4
1 -1 1 1
-1 1 -1 1
1 -1 1 1
```




```output1
NO
YES
YES
YES
NO
```



## Note

<p>One possible path for the fourth test case is given in the picture in the statement.</p>
