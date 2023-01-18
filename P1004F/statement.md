## Description

<div><p>Sonya has an array $a_1, a_2, \ldots, a_n$ consisting of $n$ integers and also one non-negative integer $x$. She has to perform $m$ queries of two types:</p><ul> <li> $1$ $i$ $y$: replace $i$-th element by value $y$, i.e. to perform an operation $a_{i}$ <span class="tex-font-style-tt">:=</span> $y$; </li><li> $2$ $l$ $r$: find the number of pairs ($L$, $R$) that $l\leq L\leq R\leq r$ and bitwise OR of all integers in the range $[L, R]$ is at least $x$ (note that $x$ is a constant for all queries). </li></ul><p>Can you help Sonya perform all her queries?</p><p>Bitwise OR is a binary operation on a pair of non-negative integers. To calculate the bitwise OR of two numbers, you need to write both numbers in binary notation. The result is a number, in binary, which contains a one in each digit if there is a one in the binary notation of at least one of the two numbers. For example, $10$ <span class="tex-font-style-tt">OR</span> $19$ = $1010_2$ <span class="tex-font-style-tt">OR</span> $10011_2$ = $11011_2$ = $27$.</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$, and $x$ ($1\leq n, m\leq 10^5$, $0\leq x&lt;2^{20}$)&nbsp;— the number of numbers, the number of queries, and the constant for all queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0\leq a_i&lt;2^{20}$)&nbsp;— numbers of the array.</p><p>The following $m$ lines each describe an query. A line has one of the following formats:</p><ul> <li> $1$ $i$ $y$ ($1\leq i\leq n$, $0\leq y&lt;2^{20}$), meaning that you have to replace $a_{i}$ by $y$; </li><li> $2$ $l$ $r$ ($1\leq l\leq r\leq n$), meaning that you have to find the number of subarrays on the segment from $l$ to $r$ that the bitwise OR of all numbers there is at least $x$. </li></ul></div><div class="output-specification"><p>For each query of type 2, print the number of subarrays such that the bitwise OR of all the numbers in the range is at least $x$.</p></div>

## Input

<p>The first line contains three integers $n$, $m$, and $x$ ($1\leq n, m\leq 10^5$, $0\leq x&lt;2^{20}$)&nbsp;— the number of numbers, the number of queries, and the constant for all queries.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0\leq a_i&lt;2^{20}$)&nbsp;— numbers of the array.</p><p>The following $m$ lines each describe an query. A line has one of the following formats:</p><ul> <li> $1$ $i$ $y$ ($1\leq i\leq n$, $0\leq y&lt;2^{20}$), meaning that you have to replace $a_{i}$ by $y$; </li><li> $2$ $l$ $r$ ($1\leq l\leq r\leq n$), meaning that you have to find the number of subarrays on the segment from $l$ to $r$ that the bitwise OR of all numbers there is at least $x$. </li></ul>

## Output

<p>For each query of type 2, print the number of subarrays such that the bitwise OR of all the numbers in the range is at least $x$.</p>





```input1
4 8 7
0 3 6 1
2 1 4
2 3 4
1 1 7
2 1 4
2 1 3
2 1 1
1 3 0
2 1 4

```




```input2
5 5 7
6 0 3 15 2
2 1 5
1 4 4
2 1 5
2 3 5
2 1 4

```




```output1
5
1
7
4
1
4

```




```output2
9
7
2
4

```



## Note

<p>In the first example, there are an array [$0$, $3$, $6$, $1$] and queries: </p><ol> <li> on the segment [$1\ldots4$], you can choose pairs ($1$, $3$), ($1$, $4$), ($2$, $3$), ($2$, $4$), and ($3$, $4$); </li><li> on the segment [$3\ldots4$], you can choose pair ($3$, $4$); </li><li> the first number is being replacing by $7$, after this operation, the array will consist of [$7$, $3$, $6$, $1$]; </li><li> on the segment [$1\ldots4$], you can choose pairs ($1$, $1$), ($1$, $2$), ($1$, $3$), ($1$, $4$), ($2$, $3$), ($2$, $4$), and ($3$, $4$); </li><li> on the segment [$1\ldots3$], you can choose pairs ($1$, $1$), ($1$, $2$), ($1$, $3$), and ($2$, $3$); </li><li> on the segment [$1\ldots1$], you can choose pair ($1$, $1$); </li><li> the third number is being replacing by $0$, after this operation, the array will consist of [$7$, $3$, $0$, $1$]; </li><li> on the segment [$1\ldots4$], you can choose pairs ($1$, $1$), ($1$, $2$), ($1$, $3$), and ($1$, $4$). </li></ol><p>In the second example, there are an array [$6$, $0$, $3$, $15$, $2$] are queries: </p><ol> <li> on the segment [$1\ldots5$], you can choose pairs ($1$, $3$), ($1$, $4$), ($1$, $5$), ($2$, $4$), ($2$, $5$), ($3$, $4$), ($3$, $5$), ($4$, $4$), and ($4$, $5$); </li><li> the fourth number is being replacing by $4$, after this operation, the array will consist of [$6$, $0$, $3$, $4$, $2$]; </li><li> on the segment [$1\ldots5$], you can choose pairs ($1$, $3$), ($1$, $4$), ($1$, $5$), ($2$, $4$), ($2$, $5$), ($3$, $4$), and ($3$, $5$); </li><li> on the segment [$3\ldots5$], you can choose pairs ($3$, $4$) and ($3$, $5$); </li><li> on the segment [$1\ldots4$], you can choose pairs ($1$, $3$), ($1$, $4$), ($2$, $4$), and ($3$, $4$). </li></ol>
