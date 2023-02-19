## Description

<div><p>We say that a sequence of $n$ integers $a_1, a_2, \ldots, a_n$ is a palindrome if for all $1 \leq i \leq n$, $a_i = a_{n-i+1}$. You are given a sequence of $n$ integers $a_1, a_2, \ldots, a_n$ and you have to find, if it exists, a <span class="tex-font-style-it">cycle permutation</span> $\sigma$ so that the sequence $a_{\sigma(1)}, a_{\sigma(2)}, \ldots, a_{\sigma(n)}$ is a palindrome. </p><p>A permutation of $1, 2, \ldots, n$ is a bijective function from $\{1, 2, \ldots, n\}$ to $\{1, 2, \ldots, n\}$. We say that a permutation $\sigma$ is a cycle permutation if $1, \sigma(1), \sigma^2(1), \ldots, \sigma^{n-1}(1)$ are pairwise different numbers. Here $\sigma^m(1)$ denotes $\underbrace{\sigma(\sigma(\ldots \sigma}_{m \text{ times}}(1) \ldots))$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 3 \cdot 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) — the size of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq n$).</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one line with <span class="tex-font-style-tt">YES</span> if a cycle permutation exists, otherwise output one line with <span class="tex-font-style-tt">NO</span>.</p><p>If the answer is <span class="tex-font-style-tt">YES</span>, output one additional line with $n$ integers $\sigma(1), \sigma(2), \ldots, \sigma(n)$, the permutation. If there is more than one permutation, you may print any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 3 \cdot 10^4$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2 \cdot 10^5$) — the size of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq n$).</p><p>The sum of $n$ for all test cases is at most $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output one line with <span class="tex-font-style-tt">YES</span> if a cycle permutation exists, otherwise output one line with <span class="tex-font-style-tt">NO</span>.</p><p>If the answer is <span class="tex-font-style-tt">YES</span>, output one additional line with $n$ integers $\sigma(1), \sigma(2), \ldots, \sigma(n)$, the permutation. If there is more than one permutation, you may print any.</p>





```input1
3
4
1 2 2 1
3
1 2 1
7
1 3 3 3 1 2 2
```




```output1
YES
3 1 4 2 
NO
YES
5 3 7 2 6 4 1
```


