## Description

<div><p>You have got a shelf and want to put some books on it.</p><p>You are given $q$ queries of three types:</p><ol> <li> <span class="tex-font-style-tt">L</span> $id$ — put a book having index $id$ on the shelf to the left from the leftmost existing book; </li><li> <span class="tex-font-style-tt">R</span> $id$ — put a book having index $id$ on the shelf to the right from the rightmost existing book; </li><li> <span class="tex-font-style-tt">?</span> $id$ — calculate the minimum number of books you need to pop from the left or from the right in such a way that the book with index $id$ will be leftmost or rightmost. </li></ol><p>You can assume that the first book you will put can have any position (it does not matter) and queries of type $3$ are always valid (it is guaranteed that the book in each such query is already placed). You can also assume that you don't put the same book on the shelf twice, so $id$s don't repeat in queries of first two types.</p><p>Your problem is to answer all the queries of type $3$ in order they appear in the input.</p><p>Note that after answering the query of type $3$ all the books remain on the shelf and the relative order of books does not change.</p><p><span class="tex-font-style-bf">If you are Python programmer, consider using PyPy instead of Python when you submit your code.</span></p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$) — the number of queries.</p><p>Then $q$ lines follow. The $i$-th line contains the $i$-th query in format as in the problem statement. It is guaranteed that queries are always valid (for query type $3$, it is guaranteed that the book in each such query is already placed, and for other types, it is guaranteed that the book was not placed before).</p><p>It is guaranteed that there is at least one query of type $3$ in the input.</p><p>In each query the constraint $1 \le id \le 2 \cdot 10^5$ is met.</p></div><div class="output-specification"><p>Print answers to queries of the type $3$ in order they appear in the input.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$) — the number of queries.</p><p>Then $q$ lines follow. The $i$-th line contains the $i$-th query in format as in the problem statement. It is guaranteed that queries are always valid (for query type $3$, it is guaranteed that the book in each such query is already placed, and for other types, it is guaranteed that the book was not placed before).</p><p>It is guaranteed that there is at least one query of type $3$ in the input.</p><p>In each query the constraint $1 \le id \le 2 \cdot 10^5$ is met.</p>

## Output

<p>Print answers to queries of the type $3$ in order they appear in the input.</p>





```input1
8
L 1
R 2
R 3
? 2
L 4
? 1
L 5
? 1

```




```input2
10
L 100
R 100000
R 123
L 101
? 123
L 10
R 115
? 100
R 110
? 115

```




```output1
1
1
2

```




```output2
0
2
1

```



## Note

<p>Let's take a look at the first example and let's consider queries: </p><ol> <li> The shelf will look like $[1]$; </li><li> The shelf will look like $[1, 2]$; </li><li> The shelf will look like $[1, 2, 3]$; </li><li> The shelf looks like $[1, \textbf{2}, 3]$ so the answer is $1$; </li><li> The shelf will look like $[4, 1, 2, 3]$; </li><li> The shelf looks like $[4, \textbf{1}, 2, 3]$ so the answer is $1$; </li><li> The shelf will look like $[5, 4, 1, 2, 3]$; </li><li> The shelf looks like $[5, 4, \textbf{1}, 2, 3]$ so the answer is $2$. </li></ol><p>Let's take a look at the second example and let's consider queries: </p><ol> <li> The shelf will look like $[100]$; </li><li> The shelf will look like $[100, 100000]$; </li><li> The shelf will look like $[100, 100000, 123]$; </li><li> The shelf will look like $[101, 100, 100000, 123]$; </li><li> The shelf looks like $[101, 100, 100000, \textbf{123}]$ so the answer is $0$; </li><li> The shelf will look like $[10, 101, 100, 100000, 123]$; </li><li> The shelf will look like $[10, 101, 100, 100000, 123, 115]$; </li><li> The shelf looks like $[10, 101, \textbf{100}, 100000, 123, 115]$ so the answer is $2$; </li><li> The shelf will look like $[10, 101, 100, 100000, 123, 115, 110]$; </li><li> The shelf looks like $[10, 101, 100, 100000, 123, \textbf{115}, 110]$ so the answer is $1$. </li></ol>
