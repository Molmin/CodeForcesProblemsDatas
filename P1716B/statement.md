## Description

<div><p>A permutation of length $n$ is a sequence of integers from $1$ to $n$ such that each integer appears in it exactly once.</p><p>Let the fixedness of a permutation $p$ be the number of fixed points in it&nbsp;— the number of positions $j$ such that $p_j = j$, where $p_j$ is the $j$-th element of the permutation $p$.</p><p>You are asked to build a sequence of permutations $a_1, a_2, \dots$, starting from the identity permutation (permutation $a_1 = [1, 2, \dots, n]$). Let's call it a permutation chain. Thus, $a_i$ is the $i$-th permutation of length $n$.</p><p>For every $i$ from $2$ onwards, the permutation $a_i$ should be obtained from the permutation $a_{i-1}$ by swapping any two elements in it (not necessarily neighboring). The fixedness of the permutation $a_i$ should be strictly lower than the fixedness of the permutation $a_{i-1}$.</p><p>Consider some chains for $n = 3$:</p><ul> <li> $a_1 = [1, 2, 3]$, $a_2 = [1, 3, 2]$&nbsp;— that is a valid chain of length $2$. From $a_1$ to $a_2$, the elements on positions $2$ and $3$ get swapped, the fixedness decrease from $3$ to $1$. </li><li> $a_1 = [2, 1, 3]$, $a_2 = [3, 1, 2]$&nbsp;— that is not a valid chain. The first permutation should always be $[1, 2, 3]$ for $n = 3$. </li><li> $a_1 = [1, 2, 3]$, $a_2 = [1, 3, 2]$, $a_3 = [1, 2, 3]$&nbsp;— that is not a valid chain. From $a_2$ to $a_3$, the elements on positions $2$ and $3$ get swapped but the fixedness increase from $1$ to $3$. </li><li> $a_1 = [1, 2, 3]$, $a_2 = [3, 2, 1]$, $a_3 = [3, 1, 2]$&nbsp;— that is a valid chain of length $3$. From $a_1$ to $a_2$, the elements on positions $1$ and $3$ get swapped, the fixedness decrease from $3$ to $1$. From $a_2$ to $a_3$, the elements on positions $2$ and $3$ get swapped, the fixedness decrease from $1$ to $0$. </li></ul><p>Find the longest permutation chain. If there are multiple longest answers, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 99$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the required length of permutations in the chain.</p></div><div class="output-specification"><p>For each testcase, first, print the length of a permutation chain $k$.</p><p>Then print $k$ permutations $a_1, a_2, \dots, a_k$. $a_1$ should be an identity permutation of length $n$ ($[1, 2, \dots, n]$). For each $i$ from $2$ to $k$, $a_i$ should be obtained by swapping two elements in $a_{i-1}$. It should also have a strictly lower fixedness than $a_{i-1}$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 99$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains a single integer $n$ ($2 \le n \le 100$)&nbsp;— the required length of permutations in the chain.</p>

## Output

<p>For each testcase, first, print the length of a permutation chain $k$.</p><p>Then print $k$ permutations $a_1, a_2, \dots, a_k$. $a_1$ should be an identity permutation of length $n$ ($[1, 2, \dots, n]$). For each $i$ from $2$ to $k$, $a_i$ should be obtained by swapping two elements in $a_{i-1}$. It should also have a strictly lower fixedness than $a_{i-1}$.</p>





```input1|2
2
2
3
```




```output1
2
1 2
2 1
3
1 2 3
3 2 1
3 1 2
```


