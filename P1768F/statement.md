## Description

<div><p>You are given an array of positive integers $a_1,a_2,\ldots,a_n$ of length $n$. </p><p>In one operation you can jump from index $i$ to index $j$ ($1 \le i \le j \le n$) by paying $\min(a_i, a_{i + 1}, \ldots, a_j) \cdot (j - i)^2$ eris.</p><p>For all $k$ from $1$ to $n$, find the minimum number of eris needed to get from index $1$ to index $k$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 4 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1,a_2,\ldots a_n$ ($1 \le a_i \le n$).</p></div><div class="output-specification"><p>Output $n$ integers&nbsp;— the $k$-th integer is the minimum number of eris needed to reach index $k$ if you start from index $1$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 4 \cdot 10^5$).</p><p>The second line contains $n$ integers $a_1,a_2,\ldots a_n$ ($1 \le a_i \le n$).</p>

## Output

<p>Output $n$ integers&nbsp;— the $k$-th integer is the minimum number of eris needed to reach index $k$ if you start from index $1$.</p>





```input1
3
2 1 3
```




```input2
6
1 4 1 6 3 2
```




```input3
2
1 2
```




```input4
4
1 4 4 4
```




```output1
0 1 2
```




```output2
0 1 2 3 6 8
```




```output3
0 1
```




```output4
0 1 4 8
```



## Note

<p>In the first example: </p><ul> <li> From $1$ to $1$: the cost is $0$, </li><li> From $1$ to $2$: $1 \rightarrow 2$ — the cost is $\min(2, 1) \cdot (2 - 1) ^ 2=1$, </li><li> From $1$ to $3$: $1 \rightarrow 2 \rightarrow 3$ — the cost is $\min(2, 1) \cdot (2 - 1) ^ 2 + \min(1, 3) \cdot (3 - 2) ^ 2 = 1 + 1 = 2$. </li></ul><p>In the fourth example from $1$ to $4$: $1 \rightarrow 3 \rightarrow 4$ — the cost is $\min(1, 4, 4) \cdot (3 - 1) ^ 2 + \min(4, 4) \cdot (4 - 3) ^ 2 = 4 + 4 = 8$.</p>
