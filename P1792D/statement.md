## Description

<div><p>You are given $n$ permutations $a_1, a_2, \dots, a_n$, each of length $m$. Recall that a permutation of length $m$ is a sequence of $m$ <span class="tex-font-style-it">distinct</span> integers from $1$ to $m$.</p><p>Let the beauty of a permutation $p_1, p_2, \dots, p_m$ be the largest $k$ such that $p_1 = 1, p_2 = 2, \dots, p_k = k$. If $p_1 \neq 1$, then the beauty is $0$.</p><p>The product of two permutations $p \cdot q$ is a permutation $r$ such that $r_j = q_{p_j}$.</p><p>For each $i$ from $1$ to $n$, print the largest beauty of a permutation $a_i \cdot a_j$ over all $j$ from $1$ to $n$ (possibly, $i = j$).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($1 \le n \le 5 \cdot 10^4$; $1 \le m \le 10$)&nbsp;— the number of permutations and the length of each permutation.</p><p>The $i$-th of the next $n$ lines contains a permutation $a_i$&nbsp;— $m$ distinct integers from $1$ to $m$.</p><p>The sum of $n$ doesn't exceed $5 \cdot 10^4$ over all testcases.</p></div><div class="output-specification"><p>For each testcase, print $n$ integers. The $i$-th value should be equal to the largest beauty of a permutation $a_i \cdot a_j$ over all $j$ ($1 \le j \le n$).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($1 \le n \le 5 \cdot 10^4$; $1 \le m \le 10$)&nbsp;— the number of permutations and the length of each permutation.</p><p>The $i$-th of the next $n$ lines contains a permutation $a_i$&nbsp;— $m$ distinct integers from $1$ to $m$.</p><p>The sum of $n$ doesn't exceed $5 \cdot 10^4$ over all testcases.</p>

## Output

<p>For each testcase, print $n$ integers. The $i$-th value should be equal to the largest beauty of a permutation $a_i \cdot a_j$ over all $j$ ($1 \le j \le n$).</p>





```input1|2,3,4,5,9,10,11,12,13,14,15,16,17
3
3 4
2 4 1 3
1 2 4 3
2 1 3 4
2 2
1 2
2 1
8 10
3 4 9 6 10 2 7 8 1 5
3 9 1 8 5 7 4 10 2 6
3 10 1 7 5 9 6 4 2 8
1 2 3 4 8 6 10 7 9 5
1 2 3 4 10 6 8 5 7 9
9 6 1 2 10 4 7 8 3 5
7 9 3 2 5 6 4 8 1 10
9 4 3 7 5 6 1 10 8 2
```




```output1
1 4 4 
2 2 
10 8 1 6 8 10 1 7
```


