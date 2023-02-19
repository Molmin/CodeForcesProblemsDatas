## Description

<div><p>A permutation $p$ of length $n$ is called <span class="tex-font-style-it">almost perfect</span> if for all integer $1 \leq i \leq n$, it holds that $\lvert p_i - p^{-1}_i \rvert \le 1$, where $p^{-1}$ is the inverse permutation of $p$ (i.e. $p^{-1}_{k_1} = k_2$ if and only if $p_{k_2} = k_1$).</p><p>Count the number of <span class="tex-font-style-it">almost perfect</span> permutations of length $n$ modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$) — the number of test cases. The description of each test case follows.</p><p>The first and only line of each test case contains a single integer $n$ ($1 \leq n \leq 3 \cdot 10^5$) — the length of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer — the number of <span class="tex-font-style-it">almost perfect</span> permutations of length $n$ modulo $998244353$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$) — the number of test cases. The description of each test case follows.</p><p>The first and only line of each test case contains a single integer $n$ ($1 \leq n \leq 3 \cdot 10^5$) — the length of the permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer — the number of <span class="tex-font-style-it">almost perfect</span> permutations of length $n$ modulo $998244353$.</p>





```input1|2,4
3
2
3
50
```




```output1
2
4
830690567
```



## Note

<p>For $n = 2$, both permutations $[1, 2]$, and $[2, 1]$ are almost perfect.</p><p>For $n = 3$, there are only $6$ permutations. Having a look at all of them gives us:</p><ul> <li> $[1, 2, 3]$ is an almost perfect permutation. </li><li> $[1, 3, 2]$ is an almost perfect permutation. </li><li> $[2, 1, 3]$ is an almost perfect permutation. </li><li> $[2, 3, 1]$ is <span class="tex-font-style-bf">NOT</span> an almost perfect permutation ($\lvert p_2 - p^{-1}_2 \rvert = \lvert 3 - 1 \rvert = 2$). </li><li> $[3, 1, 2]$ is <span class="tex-font-style-bf">NOT</span> an almost perfect permutation ($\lvert p_2 - p^{-1}_2 \rvert = \lvert 1 - 3 \rvert = 2$). </li><li> $[3, 2, 1]$ is an almost perfect permutation. </li></ul><p>So we get $4$ almost perfect permutations.</p>
