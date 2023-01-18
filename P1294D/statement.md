## Description

<div><p>Recall that <span class="tex-font-style-bf">MEX</span> of an array is a <span class="tex-font-style-bf">minimum non-negative integer</span> that does not belong to the array. Examples:</p><ul> <li> for the array $[0, 0, 1, 0, 2]$ MEX equals to $3$ because numbers $0, 1$ and $2$ are presented in the array and $3$ is the minimum non-negative integer not presented in the array; </li><li> for the array $[1, 2, 3, 4]$ MEX equals to $0$ because $0$ is the minimum non-negative integer not presented in the array; </li><li> for the array $[0, 1, 4, 3]$ MEX equals to $2$ because $2$ is the minimum non-negative integer not presented in the array. </li></ul><p>You are given an empty array $a=[]$ (in other words, a zero-length array). You are also given a positive integer $x$.</p><p>You are also given $q$ queries. The $j$-th query consists of one integer $y_j$ and means that you have to append one element $y_j$ to the array. The array length increases by $1$ after a query.</p><p>In one move, you can choose any index $i$ and set $a_i := a_i + x$ or $a_i := a_i - x$ (i.e. increase or decrease any element of the array by $x$). The only restriction is that <span class="tex-font-style-bf">$a_i$ cannot become negative</span>. Since initially the array is empty, you can perform moves only after the first query.</p><p>You have to maximize the <span class="tex-font-style-bf">MEX</span> (minimum excluded) of the array if you can perform any number of such operations (you can even perform the operation multiple times with one element).</p><p>You have to find the answer after each of $q$ queries (i.e. the $j$-th answer corresponds to the array of length $j$).</p><p><span class="tex-font-style-bf">Operations are discarded before each query. I.e. the array $a$ after the $j$-th query equals to $[y_1, y_2, \dots, y_j]$.</span></p></div><div class="input-specification"><p>The first line of the input contains two integers $q, x$ ($1 \le q, x \le 4 \cdot 10^5$) — the number of queries and the value of $x$.</p><p>The next $q$ lines describe queries. The $j$-th query consists of one integer $y_j$ ($0 \le y_j \le 10^9$) and means that you have to append one element $y_j$ to the array.</p></div><div class="output-specification"><p>Print the answer to the initial problem after each query — for the query $j$ print the maximum value of <span class="tex-font-style-bf">MEX</span> after first $j$ queries. Note that queries are dependent (the array changes after each query) but operations are independent between queries.</p></div>

## Input

<p>The first line of the input contains two integers $q, x$ ($1 \le q, x \le 4 \cdot 10^5$) — the number of queries and the value of $x$.</p><p>The next $q$ lines describe queries. The $j$-th query consists of one integer $y_j$ ($0 \le y_j \le 10^9$) and means that you have to append one element $y_j$ to the array.</p>

## Output

<p>Print the answer to the initial problem after each query — for the query $j$ print the maximum value of <span class="tex-font-style-bf">MEX</span> after first $j$ queries. Note that queries are dependent (the array changes after each query) but operations are independent between queries.</p>





```input1
7 3
0
1
2
2
0
0
10
```




```input2
4 3
1
2
1
2
```




```output1
1
2
3
3
4
4
7
```




```output2
0
0
0
0
```



## Note

<p>In the first example:</p><ul> <li> After the first query, the array is $a=[0]$: you don't need to perform any operations, maximum possible MEX is $1$. </li><li> After the second query, the array is $a=[0, 1]$: you don't need to perform any operations, maximum possible MEX is $2$. </li><li> After the third query, the array is $a=[0, 1, 2]$: you don't need to perform any operations, maximum possible MEX is $3$. </li><li> After the fourth query, the array is $a=[0, 1, 2, 2]$: you don't need to perform any operations, maximum possible MEX is $3$ (you can't make it greater with operations). </li><li> After the fifth query, the array is $a=[0, 1, 2, 2, 0]$: you can perform $a[4] := a[4] + 3 = 3$. The array changes to be $a=[0, 1, 2, 2, 3]$. Now MEX is maximum possible and equals to $4$. </li><li> After the sixth query, the array is $a=[0, 1, 2, 2, 0, 0]$: you can perform $a[4] := a[4] + 3 = 0 + 3 = 3$. The array changes to be $a=[0, 1, 2, 2, 3, 0]$. Now MEX is maximum possible and equals to $4$. </li><li> After the seventh query, the array is $a=[0, 1, 2, 2, 0, 0, 10]$. You can perform the following operations: <ul> <li> $a[3] := a[3] + 3 = 2 + 3 = 5$, </li><li> $a[4] := a[4] + 3 = 0 + 3 = 3$, </li><li> $a[5] := a[5] + 3 = 0 + 3 = 3$, </li><li> $a[5] := a[5] + 3 = 3 + 3 = 6$, </li><li> $a[6] := a[6] - 3 = 10 - 3 = 7$, </li><li> $a[6] := a[6] - 3 = 7 - 3 = 4$. </li></ul> The resulting array will be $a=[0, 1, 2, 5, 3, 6, 4]$. Now MEX is maximum possible and equals to $7$. </li></ul>
