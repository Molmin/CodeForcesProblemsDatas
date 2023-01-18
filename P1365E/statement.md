## Description

<div><p>Ridhiman challenged Ashish to find the maximum valued subsequence of an array $a$ of size $n$ consisting of positive integers. </p><p>The value of a non-empty subsequence of $k$ elements of $a$ is defined as $\sum 2^i$ over all integers $i \ge 0$ such that at least $\max(1, k - 2)$ elements of the subsequence have the $i$-th bit set in their binary representation (value $x$ has the $i$-th bit set in its binary representation if $\lfloor \frac{x}{2^i} \rfloor \mod 2$ is equal to $1$). </p><p>Recall that $b$ is a subsequence of $a$, if $b$ can be obtained by deleting some(possibly zero) elements from $a$.</p><p>Help Ashish find the maximum value he can get by choosing some subsequence of $a$.</p></div><div class="input-specification"><p>The first line of the input consists of a single integer $n$ $(1 \le n \le 500)$&nbsp;— the size of $a$.</p><p>The next line consists of $n$ space-separated integers&nbsp;— the elements of the array $(1 \le a_i \le 10^{18})$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum value Ashish can get by choosing some subsequence of $a$.</p></div>

## Input

<p>The first line of the input consists of a single integer $n$ $(1 \le n \le 500)$&nbsp;— the size of $a$.</p><p>The next line consists of $n$ space-separated integers&nbsp;— the elements of the array $(1 \le a_i \le 10^{18})$.</p>

## Output

<p>Print a single integer&nbsp;— the maximum value Ashish can get by choosing some subsequence of $a$.</p>





```input1
3
2 1 3
```




```input2
3
3 1 4
```




```input3
1
1
```




```input4
4
7 7 1 1
```




```output1
3
```




```output2
7
```




```output3
1
```




```output4
7
```



## Note

<p>For the first test case, Ashish can pick the subsequence $\{{2, 3}\}$ of size $2$. The binary representation of $2$ is <span class="tex-font-style-tt">10</span> and that of $3$ is <span class="tex-font-style-tt">11</span>. Since $\max(k - 2, 1)$ is equal to $1$, the value of the subsequence is $2^0 + 2^1$ (both $2$ and $3$ have $1$-st bit set in their binary representation and $3$ has $0$-th bit set in its binary representation). Note that he could also pick the subsequence $\{{3\}}$ or $\{{2, 1, 3\}}$.</p><p>For the second test case, Ashish can pick the subsequence $\{{3, 4\}}$ with value $7$.</p><p>For the third test case, Ashish can pick the subsequence $\{{1\}}$ with value $1$.</p><p>For the fourth test case, Ashish can pick the subsequence $\{{7, 7\}}$ with value $7$.</p>
