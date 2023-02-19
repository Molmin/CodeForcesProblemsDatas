## Description

<div><p>An integer array $a$ of length $n$ is said to be a PalindORme if ($a_{1}$ $|$ $a_{2} $ $|$ $ \ldots $ $|$ $ a_{i}) = (a_{{n - i + 1}} $ $|$ $ \ldots $ $|$ $ a_{{n - 1}} $ $|$ $ a_{n}) $ <span class="tex-font-style-bf">for all</span> $ 1 \leq i \leq n$, where $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>.</p><p>An integer array $a$ of length $n$ is considered to be good if its elements can be rearranged to form a PalindORme. Formally, array $a$ is good if there exists a permutation $p_1, p_2, \ldots p_n$ (an array where each integer from $1$ to $n$ appears exactly once) for which $a_{p_1}, a_{p_2}, \ldots a_{p_n}$ is a PalindORme.</p><p>Find the number of good arrays of length $n$, consisting only of integers in the range $[0, 2^{k} - 1]$, and print it modulo some prime $m$.</p><p>Two arrays $a_1, a_2, \ldots, a_n$ and $b_1, b_2, \ldots, b_n$ are considered to be different if there exists any $i$ $(1 \leq i \leq n)$ such that $a_i \ne b_i$.</p></div><div class="input-specification"><p>The first and only line of the input contains three integers $n$, $k$ and $m$ ($1 \leq n,k \leq 80$, $10^8 \lt m \lt 10^9$). It is guaranteed that $m$ is prime.</p></div><div class="output-specification"><p>Print a single integer &nbsp;— the number of good arrays modulo $m$.</p></div>

## Input

<p>The first and only line of the input contains three integers $n$, $k$ and $m$ ($1 \leq n,k \leq 80$, $10^8 \lt m \lt 10^9$). It is guaranteed that $m$ is prime.</p>

## Output

<p>Print a single integer &nbsp;— the number of good arrays modulo $m$.</p>





```input1
1 1 998244353
```




```input2
3 2 999999733
```




```input3
7 3 796735397
```




```input4
2 46 606559127
```




```output1
2
```




```output2
40
```




```output3
1871528
```




```output4
177013
```



## Note

<p>In the first sample, both the possible arrays $[0]$ and $[1]$ are good.</p><p>In the second sample, some examples of good arrays are:</p><ul><li> $[2, 1, 2]$ because it is already PalindORme.</li><li> $[1, 1, 0]$ because it can rearranged to $[1, 0, 1]$ which is PalindORme</li></ul><p>Note that $[1, 1, 0]$, $[1, 0, 1]$ and $[0, 1, 1]$ are all good arrays and are considered to be different according to the definition in the statement.</p><p>In the third sample, an example of a good array is $[1, 0, 1, 4, 2, 5, 4]$. It can be rearranged to an array $b = [1, 5, 0, 2, 4, 4, 1]$ which is a PalindORme because:</p><ul><li> $\mathrm{OR}(1, 1)$ = $\mathrm{OR}(7, 7)$ = $1$</li><li> $\mathrm{OR}(1, 2)$ = $\mathrm{OR}(6, 7)$ = $5$</li><li> $\mathrm{OR}(1, 3)$ = $\mathrm{OR}(5, 7)$ = $5$</li><li> $\mathrm{OR}(1, 4)$ = $\mathrm{OR}(4, 7)$ = $7$</li><li> $\mathrm{OR}(1, 5)$ = $\mathrm{OR}(3, 7)$ = $7$</li><li> $\mathrm{OR}(1, 6)$ = $\mathrm{OR}(2, 7)$ = $7$</li><li> $\mathrm{OR}(1, 7)$ = $\mathrm{OR}(1, 7)$ = $7$</li></ul><p>Here $\mathrm{OR}(l, r)$ denotes $b_{l}$ $|$ $b_{l+1} $ $|$ $ \ldots $ $|$ $ b_{r}$</p>
