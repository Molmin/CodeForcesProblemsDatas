## Description

<div><p>You are given a permutation$^\dagger$ $p$ of length $n$.</p><p>In one operation, you can choose two indices $1 \le i &lt; j \le n$ and swap $p_i$ with $p_j$.</p><p>Find the minimum number of operations needed to have <span class="tex-font-style-bf">exactly one</span> inversion$^\ddagger$ in the permutation.</p><p>$^\dagger$ A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>$^\ddagger$ The number of inversions of a permutation $p$ is the number of pairs of indices $(i, j)$ such that $1 \le i &lt; j \le n$ and $p_i &gt; p_j$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $p_1,p_2,\ldots, p_n$ ($1 \le p_i \le n$). It is guaranteed that $p$ is a permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer&nbsp;— the minimum number of operations needed to have exactly one inversion in the permutation. It can be proven that an answer always exists.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $p_1,p_2,\ldots, p_n$ ($1 \le p_i \le n$). It is guaranteed that $p$ is a permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output a single integer&nbsp;— the minimum number of operations needed to have exactly one inversion in the permutation. It can be proven that an answer always exists.</p>





```input1|2,3,6,7
4
2
2 1
2
1 2
4
3 4 1 2
4
2 4 3 1
```




```output1
0
1
3
1
```



## Note

<p>In the first test case, the permutation already satisfies the condition.</p><p>In the second test case, you can perform the operation with $(i,j)=(1,2)$, after that the permutation will be $[2,1]$ which has exactly one inversion.</p><p>In the third test case, it is not possible to satisfy the condition with less than $3$ operations. However, if we perform $3$ operations with $(i,j)$ being $(1,3)$,$(2,4)$, and $(3,4)$ in that order, the final permutation will be $[1, 2, 4, 3]$ which has exactly one inversion.</p><p>In the fourth test case, you can perform the operation with $(i,j)=(2,4)$, after that the permutation will be $[2,1,3,4]$ which has exactly one inversion.</p>
