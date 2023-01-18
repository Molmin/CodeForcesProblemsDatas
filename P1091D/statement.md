## Description

<div><p>Let $n$ be an integer. Consider all permutations on integers $1$ to $n$ in lexicographic order, and concatenate them into one big sequence $p$. For example, if $n = 3$, then $p = [1, 2, 3, 1, 3, 2, 2, 1, 3, 2, 3, 1, 3, 1, 2, 3, 2, 1]$. The length of this sequence will be $n \cdot n!$.</p><p>Let $1 \leq i \leq j \leq n \cdot n!$ be a pair of indices. We call the sequence $(p_i, p_{i+1}, \dots, p_{j-1}, p_j)$ a <span class="tex-font-style-bf">subarray</span> of $p$. Its <span class="tex-font-style-bf">length</span> is defined as the number of its elements, i.e., $j - i + 1$. Its <span class="tex-font-style-bf">sum</span> is the sum of all its elements, i.e., $\sum_{k=i}^j p_k$. </p><p>You are given $n$. Find the number of subarrays of $p$ of length $n$ having sum $\frac{n(n+1)}{2}$. Since this number may be large, output it modulo $998244353$ (a prime number). </p></div><div class="input-specification"><p>The only line contains one integer $n$&nbsp;($1 \leq n \leq 10^6$), as described in the problem statement.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of subarrays of length $n$ having sum $\frac{n(n+1)}{2}$, modulo $998244353$.</p></div>

## Input

<p>The only line contains one integer $n$&nbsp;($1 \leq n \leq 10^6$), as described in the problem statement.</p>

## Output

<p>Output a single integer&nbsp;— the number of subarrays of length $n$ having sum $\frac{n(n+1)}{2}$, modulo $998244353$.</p>





```input1
3
```




```input2
4
```




```input3
10
```




```output1
9
```




```output2
56
```




```output3
30052700
```



## Note

<p>In the first sample, there are $16$ subarrays of length $3$. In order of appearance, they are:</p><p>$[1, 2, 3]$, $[2, 3, 1]$, $[3, 1, 3]$, $[1, 3, 2]$, $[3, 2, 2]$, $[2, 2, 1]$, $[2, 1, 3]$, $[1, 3, 2]$, $[3, 2, 3]$, $[2, 3, 1]$, $[3, 1, 3]$, $[1, 3, 1]$, $[3, 1, 2]$, $[1, 2, 3]$, $[2, 3, 2]$, $[3, 2, 1]$. </p><p>Their sums are $6$, $6$, $7$, $6$, $7$, $5$, $6$, $6$, $8$, $6$, $7$, $5$, $6$, $6$, $7$, $6$. As $\frac{n(n+1)}{2} = 6$, the answer is $9$.</p>
