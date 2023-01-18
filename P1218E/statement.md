## Description

<div><p>While roaming the mystic areas of Stonefalls, in order to drop legendary loot, an adventurer was given a quest as follows. He was given an array $A = {a_1,a_2,...,a_N }$ of length $N$, and a number $K$.</p><p>Define array $B$ as $B(q, A) = $ { $q-a_1, q-a_2, ..., q-a_N$ }. Define function $F$ as $F(B,K)$ being sum of products of all $K$-tuples of elements in array $B$. For example, if the array $B$ is $[2,3,4,5]$, and with $K=3$, sum of products of all 3-tuples is $$F(B, 3) = 2*3*4+2*3*5+3*4*5+2*4*5$$</p><p>He was then given a number Q, number of queries of two types: </p><ul> <li> Type 1: Given $q$, $i$, and $d$ calculate $F(B(q, A), K)$ where we make change to initial array as $A[i] = d$. </li><li> Type 2: Given $q$, $L$, $R$, and $d$ calculate $F(B(q, A), K)$ where we make change to initial array as $A[i] = A[i] + d$ for all $i$ in range $[L, R]$ inclusive. </li></ul><p>All changes are temporarily made to initial array, and don't propagate to following queries. Help the adventurer calculate the answer to a quest, and finally get that loot!</p></div><div class="input-specification"><p>In the first two lines, numbers $N$ ($1 \leq N \leq 2*10^4$) and $K$ ($1 \leq K \leq N$), the length of initial array $A$, and tuple size, followed by $a_1,a_2,a_3,…,a_N$ ($0 \leq a_i \leq 10^9$) , elements of array $A$, in the next line. Then follows number $Q$ ($Q \leq 10$), number of queries. In the next $Q$ lines come queries of the form: </p><ul> <li> 1 q i d, for type 1, </li><li> 2 q L R d, for type 2, </li></ul><p>as explained above ($0 \leq q, d \leq 10^9, 1 \leq i,L,R \leq N$)</p></div><div class="output-specification"><p>Print $Q$ lines, the answers to queries, modulo $998244353$.</p></div>

## Input

<p>In the first two lines, numbers $N$ ($1 \leq N \leq 2*10^4$) and $K$ ($1 \leq K \leq N$), the length of initial array $A$, and tuple size, followed by $a_1,a_2,a_3,…,a_N$ ($0 \leq a_i \leq 10^9$) , elements of array $A$, in the next line. Then follows number $Q$ ($Q \leq 10$), number of queries. In the next $Q$ lines come queries of the form: </p><ul> <li> 1 q i d, for type 1, </li><li> 2 q L R d, for type 2, </li></ul><p>as explained above ($0 \leq q, d \leq 10^9, 1 \leq i,L,R \leq N$)</p>

## Output

<p>Print $Q$ lines, the answers to queries, modulo $998244353$.</p>





```input1
5
2
1 2 3 4 5
3
1 6 1 1
1 6 5 2
2 6 2 3 1
```




```output1
85
127
63
```



## Note

<p>In the first query array A = [1, 2, 3, 4, 5], B = [5, 4, 3, 2, 1], sum of products of 2-tuples = 85.</p><p>In second query array A = [1, 2, 3, 4, 2], B = [5, 4, 3, 2, 4], sum of products of 2-tuples = 127</p><p>In third query array A = [1, 3, 4, 4, 5], B = [5, 3, 2, 2, 1], sum of products of 2-tuples = 63</p>
