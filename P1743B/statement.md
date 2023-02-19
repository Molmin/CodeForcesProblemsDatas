## Description

<div><p>You are given an integer $n$. You have to construct a permutation of size $n$.</p><p>A <span class="tex-font-style-bf">permutation</span> is an array where each integer from $1$ to $s$ (where $s$ is the size of permutation) occurs exactly once. For example, $[2, 1, 4, 3]$ is a permutation of size $4$; $[1, 2, 4, 5, 3]$ is a permutation of size $5$; $[1, 4, 3]$ is not a permutation (the integer $2$ is absent), $[2, 1, 3, 1]$ is not a permutation (the integer $1$ appears twice).</p><p>A <span class="tex-font-style-bf">subsegment</span> of a permutation is a contiguous subsequence of that permutation. For example, the permutation $[2, 1, 4, 3]$ has $10$ subsegments: $[2]$, $[2, 1]$, $[2, 1, 4]$, $[2, 1, 4, 3]$, $[1]$, $[1, 4]$, $[1, 4, 3]$, $[4]$, $[4, 3]$ and $[3]$.</p><p>The <span class="tex-font-style-bf">value</span> of the permutation is the number of its subsegments which are also permutations. For example, the value of $[2, 1, 4, 3]$ is $3$ since the subsegments $[2, 1]$, $[1]$ and $[2, 1, 4, 3]$ are permutations.</p><p>You have to construct a permutation of size $n$ with <span class="tex-font-style-bf">minimum possible value</span> among all permutations of size $n$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 48$) — the number of test cases.</p><p>Then, $t$ lines follow. The $i$-th of them contains one integer $n$ ($3 \le n \le 50$) representing the $i$-th test case.</p></div><div class="output-specification"><p>For each test case, print $n$ integers — the permutation of size $n$ with <span class="tex-font-style-bf">minimum possible value</span>. If there are multiple such permutations, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 48$) — the number of test cases.</p><p>Then, $t$ lines follow. The $i$-th of them contains one integer $n$ ($3 \le n \le 50$) representing the $i$-th test case.</p>

## Output

<p>For each test case, print $n$ integers — the permutation of size $n$ with <span class="tex-font-style-bf">minimum possible value</span>. If there are multiple such permutations, print any of them.</p>





```input1|2
2
5
6
```




```output1
1 4 3 5 2
4 1 6 2 5 3
```



## Note

<p>In the first example, the permutation $[1, 4, 3, 5, 2]$ is one of the possible answers; its value is $2$.</p><p>In the second example, the permutation $[4, 1, 6, 2, 5, 3]$ is one of the possible answers; its value is $2$.</p>
