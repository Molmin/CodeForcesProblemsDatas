## Description

<div><p>Today is the final contest of INOI (Iranian National Olympiad in Informatics). The contest room is a row with $n$ computers. All computers are numbered with integers from $1$ to $n$ from left to right. There are $m$ participants, numbered with integers from $1$ to $m$.</p><p>We have an array $a$ of length $m$ where $a_{i}$ ($1 \leq a_i \leq n$) is the computer behind which the $i$-th participant wants to sit.</p><p>Also, we have another array $b$ of length $m$ consisting of characters '<span class="tex-font-style-tt">L</span>' and '<span class="tex-font-style-tt">R</span>'. $b_i$ is the side from which the $i$-th participant enters the room. '<span class="tex-font-style-tt">L</span>' means the participant enters from the left of computer $1$ and goes from left to right, and '<span class="tex-font-style-tt">R</span>' means the participant enters from the right of computer $n$ and goes from right to left.</p><p>The participants in the order from $1$ to $m$ enter the room one by one. The $i$-th of them enters the contest room in the direction $b_i$ and goes to sit behind the $a_i$-th computer. If it is occupied he keeps walking in his direction until he reaches the first unoccupied computer. After that, he sits behind it. If he doesn't find any computer he gets upset and gives up on the contest.</p><p>The madness of the $i$-th participant is the distance between his assigned computer ($a_i$) and the computer he ends up sitting behind. The distance between computers $i$ and $j$ is equal to $|i - j|$.</p><p>The values in the array $a$ <span class="tex-font-style-bf">can be</span> equal. There exist $n^m \cdot 2^m$ possible pairs of arrays $(a, b)$.</p><p>Consider all pairs of arrays $(a, b)$ such that no person becomes upset. For each of them let's calculate the sum of participants madnesses. Find the sum of all these values.</p><p>You will be given some prime modulo $p$. Find this sum by modulo $p$.</p></div><div class="input-specification"><p>The only line contains three integers $n$, $m$, $p$ ($1 \leq m \leq n \leq 500, 10^8 \leq p \leq 10 ^ 9 + 9$).</p><p>It is guaranteed, that the number $p$ is prime.</p></div><div class="output-specification"><p>Print only one integer&nbsp;— the required sum by modulo $p$.</p></div>

## Input

<p>The only line contains three integers $n$, $m$, $p$ ($1 \leq m \leq n \leq 500, 10^8 \leq p \leq 10 ^ 9 + 9$).</p><p>It is guaranteed, that the number $p$ is prime.</p>

## Output

<p>Print only one integer&nbsp;— the required sum by modulo $p$.</p>





```input1
3 1 1000000007
```




```input2
2 2 1000000009
```




```input3
3 2 998244353
```




```input4
20 10 1000000009
```




```output1
0
```




```output2
4
```




```output3
8
```




```output4
352081045
```



## Note

<p>In the first test, there are three possible arrays $a$: $\{1\}$, $\{2\}$, and $ \{3\}$ and two possible arrays $b$: $\{\mathtt{L}\}$ and $\{\mathtt{R}\}$. For all six pairs of arrays $(a, b)$, the only participant will sit behind the computer $a_1$, so his madness will be $0$. So the total sum of madnesses will be $0$.</p><p>In the second test, all possible pairs of arrays $(a, b)$, such that no person becomes upset are:</p><ul> <li> $(\{1, 1\}, \{\mathtt{L}, \mathtt{L}\})$, the sum of madnesses is $1$; </li><li> $(\{1, 1\}, \{\mathtt{R}, \mathtt{L}\})$, the sum of madnesses is $1$; </li><li> $(\{2, 2\}, \{\mathtt{R}, \mathtt{R}\})$, the sum of madnesses is $1$; </li><li> $(\{2, 2\}, \{\mathtt{L}, \mathtt{R}\})$, the sum of madnesses is $1$; </li><li> all possible pairs of $a \in \{\{1, 2\}, \{2, 1\}\}$ and $b \in \{\{\mathtt{L}, \mathtt{L}\}, \{\mathtt{R}, \mathtt{L}\}, \{\mathtt{L}, \mathtt{R}\}, \{\mathtt{R}, \mathtt{R}\}\}$, the sum of madnesses is $0$. </li></ul><p>So, the answer is $1 + 1 + 1 + 1 + 0 \ldots = 4$.</p>
