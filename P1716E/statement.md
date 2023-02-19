## Description

<div><p>You are given an array of length $2^n$. The elements of the array are numbered from $1$ to $2^n$.</p><p>You have to process $q$ queries to this array. In the $i$-th query, you will be given an integer $k$ ($0 \le k \le n-1$). To process the query, you should do the following:</p><ul> <li> for every $i \in [1, 2^n-2^k]$ <span class="tex-font-style-bf">in ascending order</span>, do the following: if the $i$-th element was already swapped with some other element <span class="tex-font-style-bf">during this query</span>, skip it; otherwise, swap $a_i$ and $a_{i+2^k}$; </li><li> after that, print the maximum sum over all contiguous subsegments of the array (including the empty subsegment). </li></ul><p>For example, if the array $a$ is $[-3, 5, -3, 2, 8, -20, 6, -1]$, and $k = 1$, the query is processed as follows:</p><ul> <li> the $1$-st element wasn't swapped yet, so we swap it with the $3$-rd element; </li><li> the $2$-nd element wasn't swapped yet, so we swap it with the $4$-th element; </li><li> the $3$-rd element was swapped already; </li><li> the $4$-th element was swapped already; </li><li> the $5$-th element wasn't swapped yet, so we swap it with the $7$-th element; </li><li> the $6$-th element wasn't swapped yet, so we swap it with the $8$-th element. </li></ul><p>So, the array becomes $[-3, 2, -3, 5, 6, -1, 8, -20]$. The subsegment with the maximum sum is $[5, 6, -1, 8]$, and the answer to the query is $18$.</p><p>Note that the queries actually <span class="tex-font-style-bf">change the array</span>, i. e. after a query is performed, the array does not return to its original state, and the next query will be applied to the modified array.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 18$).</p><p>The second line contains $2^n$ integers $a_1, a_2, \dots, a_{2^n}$ ($-10^9 \le a_i \le 10^9$).</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$).</p><p>Then $q$ lines follow, the $i$-th of them contains one integer $k$ ($0 \le k \le n-1$) describing the $i$-th query.</p></div><div class="output-specification"><p>For each query, print one integer&nbsp;— the maximum sum over all contiguous subsegments of the array (including the empty subsegment) after processing the query.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 18$).</p><p>The second line contains $2^n$ integers $a_1, a_2, \dots, a_{2^n}$ ($-10^9 \le a_i \le 10^9$).</p><p>The third line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$).</p><p>Then $q$ lines follow, the $i$-th of them contains one integer $k$ ($0 \le k \le n-1$) describing the $i$-th query.</p>

## Output

<p>For each query, print one integer&nbsp;— the maximum sum over all contiguous subsegments of the array (including the empty subsegment) after processing the query.</p>





```input1
3
-3 5 -3 2 8 -20 6 -1
3
1
0
1
```




```output1
18
8
13
```



## Note

<p>Transformation of the array in the example: $[-3, 5, -3, 2, 8, -20, 6, -1] \rightarrow [-3, 2, -3, 5, 6, -1, 8, -20] \rightarrow [2, -3, 5, -3, -1, 6, -20, 8] \rightarrow [5, -3, 2, -3, -20, 8, -1, 6]$.</p>
