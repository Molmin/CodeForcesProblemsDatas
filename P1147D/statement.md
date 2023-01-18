## Description

<div><p>You are given a string $s$ consisting of characters "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">0</span>", and "<span class="tex-font-style-tt">?</span>". The first character of $s$ is guaranteed to be "<span class="tex-font-style-tt">1</span>". Let $m$ be the number of characters in $s$.</p><p>Count the number of ways we can choose a pair of integers $a, b$ that satisfies the following: </p><ul> <li> $1 \leq a &lt; b &lt; 2^m$ </li><li> When written without leading zeros, the base-2 representations of $a$ and $b$ are both palindromes. </li><li> The base-2 representation of <span class="tex-font-style-tt">bitwise XOR</span> of $a$ and $b$ matches the pattern $s$. We say that $t$ matches $s$ if the lengths of $t$ and $s$ are the same and for every $i$, the $i$-th character of $t$ is equal to the $i$-th character of $s$, or the $i$-th character of $s$ is "<span class="tex-font-style-tt">?</span>". </li></ul><p>Compute this count modulo $998244353$. </p></div><div class="input-specification"><p>The first line contains a single string $s$ ($1 \leq |s| \leq 1\,000$). $s$ consists only of characters "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">?</span>". It is guaranteed that the first character of $s$ is a "<span class="tex-font-style-tt">1</span>".</p></div><div class="output-specification"><p>Print a single integer, the count of pairs that satisfy the conditions modulo $998244353$.</p></div>

## Input

<p>The first line contains a single string $s$ ($1 \leq |s| \leq 1\,000$). $s$ consists only of characters "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">?</span>". It is guaranteed that the first character of $s$ is a "<span class="tex-font-style-tt">1</span>".</p>

## Output

<p>Print a single integer, the count of pairs that satisfy the conditions modulo $998244353$.</p>





```input1
10110
```




```input2
1?0???10
```




```input3
1?????????????????????????????????????
```




```input4
1
```




```output1
3
```




```output2
44
```




```output3
519569202
```




```output4
0
```



## Note

<p>For the first example, the pairs in base-2 are $(111, 10001), (11, 10101), (1001, 11111)$.</p>
