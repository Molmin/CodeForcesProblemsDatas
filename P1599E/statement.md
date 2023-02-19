## Description

<div><p>You are given two integer arrays of length $N$, $A1$ and $A2$. You are also given $Q$ queries of 4 types: </p><p>1 k l r x: set $Ak_i:=min(Ak_i, x)$ for each $l \leq i \leq r$.</p><p>2 k l r x: set $Ak_i:=max(Ak_i, x)$ for each $l \leq i \leq r$.</p><p>3 k l r x: set $Ak_i:=Ak_i+x$ for each $l \leq i \leq r$.</p><p>4 l r: find the $(\sum_{i=l}^r F(A1_i+A2_i)) \% (10^9+7)$ where $F(k)$ is the $k$-th Fibonacci number ($F(0)=0, F(1)=1, F(k)=F(k-1)+F(k-2)$), and $x \% y$ denotes the remainder of the division of $x$ by $y$.</p><p>You should process these queries and answer each query of the fourth type.</p></div><div class="input-specification"><p>The first line contains two integers $N$ and $Q$. ($1 \leq N, Q \leq 5 \times 10^4$) </p><p>The second line contains $N$ integers, array $A1_1, A1_2, \dots A1_N$. ($0 \leq A1_i \leq 10^6$)</p><p>The third line contains $N$ integers, array $A2_1, A2_2, \dots A2_N$. ($0 \leq A2_i \leq 10^6$)</p><p>The next $Q$ lines describe the queries. Each line contains 5 or 3 integers, where the first integer denotes the type of the query. ($k \in \{1, 2\}$, $1 \leq l \leq r \leq N$)</p><p>For queries of type 1 and 2, $0 \leq x \leq 10^9$ holds.</p><p>For queries of type 3, $−10^6 \leq x \leq 10^6$ holds.</p><p>It is guaranteed that after every query each number in arrays $A1$ and $A2$ will be nonnegative. </p></div><div class="output-specification"><p>Print the answer to each query of the fourth type, in separate lines. </p></div>

## Input

<p>The first line contains two integers $N$ and $Q$. ($1 \leq N, Q \leq 5 \times 10^4$) </p><p>The second line contains $N$ integers, array $A1_1, A1_2, \dots A1_N$. ($0 \leq A1_i \leq 10^6$)</p><p>The third line contains $N$ integers, array $A2_1, A2_2, \dots A2_N$. ($0 \leq A2_i \leq 10^6$)</p><p>The next $Q$ lines describe the queries. Each line contains 5 or 3 integers, where the first integer denotes the type of the query. ($k \in \{1, 2\}$, $1 \leq l \leq r \leq N$)</p><p>For queries of type 1 and 2, $0 \leq x \leq 10^9$ holds.</p><p>For queries of type 3, $−10^6 \leq x \leq 10^6$ holds.</p><p>It is guaranteed that after every query each number in arrays $A1$ and $A2$ will be nonnegative. </p>

## Output

<p>Print the answer to each query of the fourth type, in separate lines. </p>





```input1
3 4
1 0 2
2 1 0
4 1 3
3 2 2 2 3
1 1 1 3 0
4 1 3
```




```input2
5 4
1 3 5 3 2
4 2 1 3 3
4 1 3
4 2 5
2 1 2 4 6
4 2 4
```




```output1
4
4
```




```output2
18
26
68
```



## Note

<p>In the first example: The answer for the first query is $F(1 + 2) + F(0 + 1) + F(2 + 0) = F(3) + F(1) + F(2) = 2 + 1 + 1 = 4$. After the second query, the array $A2$ changes to $[2, 4, 0]$. After the third query, the array $A1$ changes to $[0, 0, 0]$. The answer for the fourth query is $F(0 + 2) + F(0 + 4) + F(0 + 0) = F(2) + F(4) + F(0) = 1 + 3 + 0 = 4$. </p><p>In the second example: The answer for the first query is $F(1 + 4) + F(3 + 2) + F(5 + 1) = F(5) + F(5) + F(6) = 5 + 5 + 8 = 18$. The answer for the second query is $F(3 + 2) + F(5 + 1) + F(3 + 3) + F(2 + 3) = F(5) + F(6) + F(6) + F(5) = 5 + 8 + 8 + 5 = 26$. After the third query, the array $A1$ changes to $[1, 6, 6, 6, 2]$. The answer for the fourth query is $F(6 + 2) + F(6 + 1) + F(6 + 3) = F(8) + F(7) + F(9) = 21 + 13 + 34 = 68$. </p>
