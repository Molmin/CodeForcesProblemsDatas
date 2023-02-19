## Description

<div><p>You are given a permutation $a$ of size $n$ and you should perform $n$ operations on it. In the $i$-th operation, you can choose a non-empty suffix of $a$ and increase all of its elements by $i$. How can we perform the operations to minimize the number of inversions in the final array?</p><p>Note that you can perform operations on the same suffix any number of times you want.</p><p>A permutation of size $n$ is an array of size $n$ such that each integer from $1$ to $n$ occurs exactly once in this array. A suffix is several consecutive elements of an array that include the last element of the array. An inversion in an array $a$ is a pair of indices $(i, j)$ such that $i &gt; j$ and $a_{i} &lt; a_{j}$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the size of the array.</p><p>The second line contains $n$ distinct integers $a_{1}, a_{2}, \dots, a_{n}$ ($1 \le a_i \le n$), the initial permutation $a$.</p><p>It's guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $n$ integers $x_{1}, x_{2}, \ldots, x_{n}$ ($1 \le x_{i} \le n$ for each $1 \le i \le n$) indicating that the $i$-th operation must be applied to the suffix <span class="tex-font-style-bf">starting at index</span> $x_{i}$. If there are multiple answers, print any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) — the size of the array.</p><p>The second line contains $n$ distinct integers $a_{1}, a_{2}, \dots, a_{n}$ ($1 \le a_i \le n$), the initial permutation $a$.</p><p>It's guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $n$ integers $x_{1}, x_{2}, \ldots, x_{n}$ ($1 \le x_{i} \le n$ for each $1 \le i \le n$) indicating that the $i$-th operation must be applied to the suffix <span class="tex-font-style-bf">starting at index</span> $x_{i}$. If there are multiple answers, print any of them.</p>





```input1|2,3,6,7
4
4
1 2 3 4
5
1 3 2 4 5
3
2 3 1
1
1
```




```output1
1 1 1 1
1 4 3 2 1
1 3 3
1
```



## Note

<p>In the first test case one of the optimal solutions is to increase the whole array on each operation (that is, choose the suffix starting at index $1$). The final array $[11, 12, 13, 14]$ contains $0$ inversions.</p><p>In the second test case, $a$ will be equal to $[2, 4, 3, 5, 6]$, $[2, 4, 3, 7, 8]$, $[2, 4, 6, 10, 11]$, $[2, 8, 10, 14, 15]$ and $[7, 13, 15, 19, 20]$ after the first, second, third, fourth, and fifth operations, respectively. So the final array $a$ has zero inversions.</p>
