## Description

<div><p>You are given an integer array $a_1, a_2, \ldots, a_n$.</p><p>The array $b$ is called to be a <span class="tex-font-style-it">subsequence</span> of $a$ if it is possible to remove some elements from $a$ to get $b$.</p><p>Array $b_1, b_2, \ldots, b_k$ is called to be <span class="tex-font-style-it">good</span> if it is not empty and for every $i$ ($1 \le i \le k$) $b_i$ is divisible by $i$.</p><p>Find the number of good subsequences in $a$ modulo $10^9 + 7$. </p><p>Two subsequences are considered different if index sets of numbers included in them are different. That is, the values ​of the elements ​do not matter in the comparison of subsequences. In particular, the array $a$ has exactly $2^n - 1$ different subsequences (excluding an empty subsequence).</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 100\,000$)&nbsp;— the length of the array $a$.</p><p>The next line contains integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p></div><div class="output-specification"><p>Print exactly one integer&nbsp;— the number of good subsequences taken modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 100\,000$)&nbsp;— the length of the array $a$.</p><p>The next line contains integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^6$).</p>

## Output

<p>Print exactly one integer&nbsp;— the number of good subsequences taken modulo $10^9 + 7$.</p>





```input1
2
1 2

```




```input2
5
2 2 1 22 14

```




```output1
3
```




```output2
13
```



## Note

<p>In the first example, all three non-empty possible subsequences are good: $\{1\}$, $\{1, 2\}$, $\{2\}$</p><p>In the second example, the possible good subsequences are: $\{2\}$, $\{2, 2\}$, $\{2, 22\}$, $\{2, 14\}$, $\{2\}$, $\{2, 22\}$, $\{2, 14\}$, $\{1\}$, $\{1, 22\}$, $\{1, 14\}$, $\{22\}$, $\{22, 14\}$, $\{14\}$.</p><p>Note, that some subsequences are listed more than once, since they occur in the original array multiple times.</p>
