## Description

<div><p>There is a prison that can be represented as a rectangular matrix with $n$ rows and $m$ columns. Therefore, there are $n \cdot m$ prison cells. There are also $n \cdot m$ prisoners, one in each prison cell. Let's denote the cell in the $i$-th row and the $j$-th column as $(i, j)$.</p><p>There's a secret tunnel in the cell $(r, c)$, that the prisoners will use to escape! However, to avoid the risk of getting caught, they will escape at night.</p><p>Before the night, every prisoner is in his own cell. When night comes, they can start moving to adjacent cells. Formally, in one second, a prisoner located in cell $(i, j)$ can move to cells $( i - 1 , j )$ , $( i + 1 , j )$ , $( i , j - 1 )$ , or $( i , j + 1 )$, as long as the target cell is inside the prison. They can also choose to stay in cell $(i, j)$.</p><p>The prisoners want to know the minimum number of seconds needed so that every prisoner can arrive to cell $( r , c )$ if they move optimally. Note that there can be any number of prisoners in the same cell at the same time. </p></div><div class="input-specification"><p>The first line contains an integer $t$ $(1 \le t \le 10^4)$, the number of test cases.</p><p>Each of the next $t$ lines contains four space-separated integers $n$, $m$, $r$, $c$ ($1 \le r \le n \le 10^9$, $1 \le c \le m \le 10^9$).</p></div><div class="output-specification"><p>Print $t$ lines, the answers for each test case.</p></div>

## Input

<p>The first line contains an integer $t$ $(1 \le t \le 10^4)$, the number of test cases.</p><p>Each of the next $t$ lines contains four space-separated integers $n$, $m$, $r$, $c$ ($1 \le r \le n \le 10^9$, $1 \le c \le m \le 10^9$).</p>

## Output

<p>Print $t$ lines, the answers for each test case.</p>





```input1
3
10 10 1 1
3 5 2 4
10 2 5 1
```




```output1
18
4
6
```


