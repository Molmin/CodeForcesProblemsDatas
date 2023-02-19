## Description

<div><p>Let's say Pak Chanek has an array $A$ consisting of $N$ positive integers. Pak Chanek will do a number of operations. In each operation, Pak Chanek will do the following: </p><ol> <li> Choose an index $p$ ($1 \leq p \leq N$). </li><li> Let $c$ be the number of operations that have been done <span class="tex-font-style-bf">on index $p$</span> before this operation. </li><li> Decrease the value of $A_p$ by $2^c$. </li><li> Multiply the value of $A_p$ by $2$. </li></ol><p>After each operation, all elements of $A$ must be <span class="tex-font-style-bf">positive integers</span>.</p><p>An array $A$ is said to be sortable if and only if Pak Chanek can do zero or more operations so that $A_1 &lt; A_2 &lt; A_3 &lt; A_4 &lt; \ldots &lt; A_N$.</p><p>Pak Chanek must find an array $A$ that is sortable with length $N$ such that $A_1 + A_2 + A_3 + A_4 + \ldots + A_N$ is the minimum possible. If there are more than one possibilities, Pak Chanek must choose the array that is <span class="tex-font-style-bf">lexicographically minimum</span> among them.</p><p>Pak Chanek must solve the following things: </p><ul> <li> Pak Chanek must print the value of $A_1 + A_2 + A_3 + A_4 + \ldots + A_N$ for that array. </li><li> $Q$ questions will be given. For the $i$-th question, an integer $P_i$ is given. Pak Chanek must print the value of $A_{P_i}$. </li></ul><p>Help Pak Chanek solve the problem.</p><p>Note: an array $B$ of size $N$ is said to be lexicographically smaller than an array $C$ that is also of size $N$ if and only if there exists an index $i$ such that $B_i &lt; C_i$ and for each $j &lt; i$, $B_j = C_j$.</p></div><div class="input-specification"><p>The first line contains two integers $N$ and $Q$ ($1 \leq N \leq 10^9$, $0 \leq Q \leq \min(N, 10^5)$) — the required length of array $A$ and the number of questions.</p><p>The $i$-th of the next $Q$ lines contains a single integer $P_i$ ($1 \leq P_1 &lt; P_2 &lt; \ldots &lt; P_Q \leq N$) — the index asked in the $i$-th question.</p></div><div class="output-specification"><p>Print $Q+1$ lines. The $1$-st line contains an integer representing $A_1 + A_2 + A_3 + A_4 + \ldots + A_N$. For each $1 \leq i \leq Q$, the $(i+1)$-th line contains an integer representing $A_{P_i}$.</p></div>

## Input

<p>The first line contains two integers $N$ and $Q$ ($1 \leq N \leq 10^9$, $0 \leq Q \leq \min(N, 10^5)$) — the required length of array $A$ and the number of questions.</p><p>The $i$-th of the next $Q$ lines contains a single integer $P_i$ ($1 \leq P_1 &lt; P_2 &lt; \ldots &lt; P_Q \leq N$) — the index asked in the $i$-th question.</p>

## Output

<p>Print $Q+1$ lines. The $1$-st line contains an integer representing $A_1 + A_2 + A_3 + A_4 + \ldots + A_N$. For each $1 \leq i \leq Q$, the $(i+1)$-th line contains an integer representing $A_{P_i}$.</p>





```input1
6 3
1
4
5
```




```input2
1 0
```




```output1
17
1
3
4
```




```output2
1
```



## Note

<p>In the first example, the array $A$ obtained is $[1, 2, 3, 3, 4, 4]$. We can see that the array is sortable by doing the following operations: </p><ul> <li> Choose index $5$, then $A = [1, 2, 3, 3, 6, 4]$. </li><li> Choose index $6$, then $A = [1, 2, 3, 3, 6, 6]$. </li><li> Choose index $4$, then $A = [1, 2, 3, 4, 6, 6]$. </li><li> Choose index $6$, then $A = [1, 2, 3, 4, 6, 8]$. </li></ul>
