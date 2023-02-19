## Description

<div><p>We call an array $a$ of length $n$ <span class="tex-font-style-it">fancy</span> if for each $1 &lt; i \le n$ it holds that $a_i = a_{i-1} + 1$.</p><p>Let's call $f(p)$ applied to a permutation$^\dagger$ of length $n$ as the <span class="tex-font-style-bf">minimum</span> number of subarrays it can be partitioned such that each one of them is fancy. For example $f([1,2,3]) = 1$, while $f([3,1,2]) = 2$ and $f([3,2,1]) = 3$.</p><p>Given $n$ and a permutation $p$ of length $n$, we define a permutation $p'$ of length $n$ to be $k$-special if and only if:</p><ul> <li> $p'$ is lexicographically smaller$^\ddagger$ than $p$, and </li><li> $f(p') = k$. </li></ul><p>Your task is to count for each $1 \le k \le n$ the number of $k$-special permutations modulo $m$.</p><p>$^\dagger$ A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>$^\ddagger$ A permutation $a$ of length $n$ is lexicographically smaller than a permutation $b$ of length $n$ if and only if the following holds: in the first position where $a$ and $b$ differ, the permutation $a$ has a smaller element than the corresponding element in $b$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2000$, $10 \le m \le 10^9$) — the length of the permutation and the required modulo.</p><p>The second line contains $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$) — the permutation $p$.</p></div><div class="output-specification"><p>Print $n$ integers, where the $k$-th integer is the number of $k$-special permutations modulo $m$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2000$, $10 \le m \le 10^9$) — the length of the permutation and the required modulo.</p><p>The second line contains $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$) — the permutation $p$.</p>

## Output

<p>Print $n$ integers, where the $k$-th integer is the number of $k$-special permutations modulo $m$.</p>





```input1
4 666012
1 3 4 2
```




```input2
3 10
3 2 1
```




```input3
7 1000000000
7 2 1 3 5 4 6
```




```input4
10 11
10 9 8 7 6 5 4 3 2 1
```




```output1
1 0 1 1
```




```output2
1 2 2
```




```output3
1 6 40 201 705 1635 1854
```




```output4
1 9 9 0 1 5 5 0 1 0
```



## Note

<p>In the first example, the permutations that are lexicographically smaller than $[1,3,4,2]$ are:</p><ul> <li> $[1,2,3,4]$, $f([1,2,3,4])=1$; </li><li> $[1,2,4,3]$, $f([1,2,4,3])=3$; </li><li> $[1,3,2,4]$, $f([1,3,2,4])=4$. </li></ul><p>Thus our answer is $[1,0,1,1]$.</p><p>In the second example, the permutations that are lexicographically smaller than $[3,2,1]$ are:</p><ul> <li> $[1,2,3]$, $f([1,2,3])=1$; </li><li> $[1,3,2]$, $f([1,3,2])=3$; </li><li> $[2,1,3]$, $f([2,1,3])=3$; </li><li> $[2,3,1]$, $f([2,3,1])=2$; </li><li> $[3,1,2]$, $f([3,1,2])=2$. </li></ul><p>Thus our answer is $[1,2,2]$.</p>
