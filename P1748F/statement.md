## Description

<div><p>You have an array $a_0, a_1, \ldots, a_{n-1}$ of length $n$. Initially, $a_i = 2^i$ for all $0 \le i \lt n$. Note that array $a$ is zero-indexed. </p><p>You want to reverse this array (that is, make $a_i$ equal to $2^{n-1-i}$ for all $0 \le i \lt n$). To do this, you can perform the following operation no more than $250\,000$ times:</p><ul> <li> Select an integer $i$ ($0 \le i \lt n$) and replace $a_i$ by $a_i \oplus a_{(i+1)\bmod n}$. </li></ul><p>Here, $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Your task is to find <span class="tex-font-style-bf">any</span> sequence of operations that will result in the array $a$ being reversed. It can be shown that under the given constraints, a solution always exists.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 400$)&nbsp;— the length of the array $a$.</p></div><div class="output-specification"><p>On the first line print one integer $k$ ($0 \le k \le 250\,000$)&nbsp;— the number of operations performed.</p><p>On the second line print $k$ integers $i_1,i_2,\ldots,i_k$ ($0 \le i_j \lt n$). Here, $i_j$ should be the integer selected on the $j$-th operation.</p><p>Note that you don't need to minimize the number of operations.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 400$)&nbsp;— the length of the array $a$.</p>

## Output

<p>On the first line print one integer $k$ ($0 \le k \le 250\,000$)&nbsp;— the number of operations performed.</p><p>On the second line print $k$ integers $i_1,i_2,\ldots,i_k$ ($0 \le i_j \lt n$). Here, $i_j$ should be the integer selected on the $j$-th operation.</p><p>Note that you don't need to minimize the number of operations.</p>





```input1
2
```




```input2
3
```




```output1
3
1 0 1
```




```output2
9
1 0 1 0 2 1 0 1 0
```



## Note

<p>In the notes, the elements on which the operations are performed are colored red.</p><p>In the first test case, array $a$ will change in the following way: </p><p>$[1,\color{red}{2}] \rightarrow [\color{red}{1},3] \rightarrow [2,\color{red}{3}] \rightarrow [2,1]$.</p><p>In the second test case, array $a$ will change in the following way:</p><p>$[1,\color{red}{2},4] \rightarrow [\color{red}{1},6,4] \rightarrow [7,\color{red}{6},4] \rightarrow [\color{red}{7},2,4] \rightarrow [5,2,\color{red}{4}] \rightarrow [5,\color{red}{2},1] \rightarrow [\color{red}{5},3,1] \rightarrow [6,\color{red}{3},1] \rightarrow [\color{red}{6},2,1] \rightarrow [4,2,1]$.</p>
