## Description

<div><p>You are given a matrix consisting of $n$ rows and $m$ columns. The matrix contains lowercase letters of the Latin alphabet.</p><p>You can perform the following operation any number of times you want to: choose two integers $i$ ($1 \le i \le m$) and $k$ ($0 &lt; k &lt; n$), and shift every column $j$ such that $i \le j \le m$ cyclically by $k$. The shift is performed upwards.</p><p>For example, if you have a matrix </p><center> $\left( \begin{array} \\ a &amp; b &amp; c \\ d &amp; e &amp; f \\ g &amp; h &amp; i \end{array}\right) $ </center> and perform an operation with $i = 2$, $k = 1$, then it becomes: <center> $\left( \begin{array} \\ a &amp; e &amp; f \\ d &amp; h &amp; i \\ g &amp; b &amp; c \end{array}\right) $ </center><p>You have to process $q$ queries. Each of the queries is a string of length $m$ consisting of lowercase letters of the Latin alphabet. For each query, you have to calculate the minimum number of operations described above you have to perform so that at least one row of the matrix is equal to the string from the query. Note that all queries are independent, that is, the operations you perform in a query don't affect the initial matrix in other queries.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, $q$ ($2 \le n, m, q \le 2.5 \cdot 10^5$; $n \cdot m \le 5 \cdot 10^5$; $q \cdot m \le 5 \cdot 10^5$) — the number of rows and columns in the matrix and the number of queries, respectively.</p><p>The next $n$ lines contains $m$ lowercase Latin letters each — elements of the matrix.</p><p>The following $q$ lines contains a description of queries — strings of length $m$ consisting of lowercase letters of the Latin alphabet.</p></div><div class="output-specification"><p>Print $q$ integers. The $i$-th integer should be equal to the minimum number of operations you have to perform so that the matrix contains a string from the $i$-th query or $-1$ if the specified string cannot be obtained.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, $q$ ($2 \le n, m, q \le 2.5 \cdot 10^5$; $n \cdot m \le 5 \cdot 10^5$; $q \cdot m \le 5 \cdot 10^5$) — the number of rows and columns in the matrix and the number of queries, respectively.</p><p>The next $n$ lines contains $m$ lowercase Latin letters each — elements of the matrix.</p><p>The following $q$ lines contains a description of queries — strings of length $m$ consisting of lowercase letters of the Latin alphabet.</p>

## Output

<p>Print $q$ integers. The $i$-th integer should be equal to the minimum number of operations you have to perform so that the matrix contains a string from the $i$-th query or $-1$ if the specified string cannot be obtained.</p>





```input1
3 5 4
abacc
ccbba
ccabc
abacc
acbbc
ababa
acbbc
```




```input2
6 4 4
daac
bcba
acad
cbdc
aaaa
bcbb
dcdd
acba
bbbb
dbcd
```




```input3
5 10 5
ltjksdyfgg
cbhpsereqn
ijndtzbzcf
ghgcgeadep
bfzdgxqmqe
ibgcgzyfep
bbhdgxqmqg
ltgcgxrzep
ljnpseldgn
ghhpseyzcf
```




```output1
0
2
1
2
```




```output2
3
1
2
-1
```




```output3
5
3
5
-1
3
```


