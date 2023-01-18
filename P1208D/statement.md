## Description

<div><p>An array of integers $p_{1},p_{2}, \ldots,p_{n}$ is called a permutation if it contains each number from $1$ to $n$ exactly once. For example, the following arrays are permutations: $[3,1,2], [1], [1,2,3,4,5]$ and $[4,3,1,2]$. The following arrays are not permutations: $[2], [1,1], [2,3,4]$.</p><p>There is a hidden permutation of length $n$.</p><p>For each index $i$, you are given $s_{i}$, which equals to the sum of all $p_{j}$ such that $j &lt; i$ and $p_{j} &lt; p_{i}$. In other words, $s_i$ is the sum of elements before the $i$-th element that are smaller than the $i$-th element.</p><p>Your task is to restore the permutation.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^{5}$)&nbsp;— the size of the permutation.</p><p>The second line contains $n$ integers $s_{1}, s_{2}, \ldots, s_{n}$ ($0 \le s_{i} \le \frac{n(n-1)}{2}$).</p><p>It is guaranteed that the array $s$ corresponds to a valid permutation of length $n$.</p></div><div class="output-specification"><p>Print $n$ integers $p_{1}, p_{2}, \ldots, p_{n}$ — the elements of the restored permutation. We can show that the answer is always unique.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^{5}$)&nbsp;— the size of the permutation.</p><p>The second line contains $n$ integers $s_{1}, s_{2}, \ldots, s_{n}$ ($0 \le s_{i} \le \frac{n(n-1)}{2}$).</p><p>It is guaranteed that the array $s$ corresponds to a valid permutation of length $n$.</p>

## Output

<p>Print $n$ integers $p_{1}, p_{2}, \ldots, p_{n}$ — the elements of the restored permutation. We can show that the answer is always unique.</p>





```input1
3
0 0 0
```




```input2
2
0 1
```




```input3
5
0 1 1 1 10
```




```output1
3 2 1
```




```output2
1 2
```




```output3
1 4 3 2 5
```



## Note

<p>In the first example for each $i$ there is no index $j$ satisfying both conditions, hence $s_i$ are always $0$.</p><p>In the second example for $i = 2$ it happens that $j = 1$ satisfies the conditions, so $s_2 = p_1$.</p><p>In the third example for $i = 2, 3, 4$ only $j = 1$ satisfies the conditions, so $s_2 = s_3 = s_4 = 1$. For $i = 5$ all $j = 1, 2, 3, 4$ are possible, so $s_5 = p_1 + p_2 + p_3 + p_4 = 10$.</p>
