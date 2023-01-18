## Description

<div><p>Kuroni is the coordinator of the next Mathforces round written by the "Proof by AC" team. All the preparation has been done, and he is discussing with the team about the score distribution for the round.</p><p>The round consists of $n$ problems, numbered from $1$ to $n$. The problems are ordered in increasing order of difficulty, no two problems have the same difficulty. A score distribution for the round can be denoted by an array $a_1, a_2, \dots, a_n$, where $a_i$ is the score of $i$-th problem. </p><p>Kuroni thinks that the score distribution should satisfy the following requirements:</p><ul> <li> The score of each problem should be a positive integer not exceeding $10^9$. </li><li> A harder problem should grant a strictly higher score than an easier problem. In other words, $1 \leq a_1 &lt; a_2 &lt; \dots &lt; a_n \leq 10^9$. </li><li> The <span class="tex-font-style-bf">balance</span> of the score distribution, defined as the number of triples $(i, j, k)$ such that $1 \leq i &lt; j &lt; k \leq n$ and $a_i + a_j = a_k$, should be exactly $m$. </li></ul><p>Help the team find a score distribution that satisfies Kuroni's requirement. In case such a score distribution does not exist, output $-1$.</p></div><div class="input-specification"><p>The first and single line contains two integers $n$ and $m$ ($1 \le n \le 5000$, $0 \leq m \leq 10^9$)&nbsp;— the number of problems and the required balance.</p></div><div class="output-specification"><p>If there is no solution, print a single integer $-1$.</p><p>Otherwise, print a line containing $n$ integers $a_1, a_2, \dots, a_n$, representing a score distribution that satisfies all the requirements. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first and single line contains two integers $n$ and $m$ ($1 \le n \le 5000$, $0 \leq m \leq 10^9$)&nbsp;— the number of problems and the required balance.</p>

## Output

<p>If there is no solution, print a single integer $-1$.</p><p>Otherwise, print a line containing $n$ integers $a_1, a_2, \dots, a_n$, representing a score distribution that satisfies all the requirements. If there are multiple answers, print any of them.</p>





```input1
5 3
```




```input2
8 0
```




```input3
4 10
```




```output1
4 5 9 13 18
```




```output2
10 11 12 13 14 15 16 17
```




```output3
-1
```



## Note

<p>In the first example, there are $3$ triples $(i, j, k)$ that contribute to the balance of the score distribution. </p><ul> <li> $(1, 2, 3)$ </li><li> $(1, 3, 4)$ </li><li> $(2, 4, 5)$ </li></ul>
