## Description

<div><p>For an array $[b_1, b_2, \ldots, b_m]$ define its number of inversions as the number of pairs $(i, j)$ of integers such that $1 \le i &lt; j \le m$ and $b_i&gt;b_j$. Let's call array $b$ <span class="tex-font-style-bf">odd</span> if its number of inversions is odd. </p><p>For example, array $[4, 2, 7]$ is odd, as its number of inversions is $1$, while array $[2, 1, 4, 3]$ isn't, as its number of inversions is $2$.</p><p>You are given a permutation $[p_1, p_2, \ldots, p_n]$ of integers from $1$ to $n$ (each of them appears exactly once in the permutation). You want to split it into several consecutive subarrays (maybe just one), so that the number of the <span class="tex-font-style-bf">odd</span> subarrays among them is as large as possible. </p><p>What largest number of these subarrays may be <span class="tex-font-style-bf">odd</span>?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) &nbsp;— the size of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct) &nbsp;— the elements of the permutation.</p><p>The sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer &nbsp;— the largest possible number of <span class="tex-font-style-bf">odd</span> subarrays that you can get after splitting the permutation into several consecutive subarrays.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$) &nbsp;— the size of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, all $p_i$ are distinct) &nbsp;— the elements of the permutation.</p><p>The sum of $n$ over all test cases doesn't exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case output a single integer &nbsp;— the largest possible number of <span class="tex-font-style-bf">odd</span> subarrays that you can get after splitting the permutation into several consecutive subarrays.</p>





```input1
5
3
1 2 3
4
4 3 2 1
2
1 2
2
2 1
6
4 5 6 1 2 3
```




```output1
0
2
0
1
1
```



## Note

<p>In the first and third test cases, no matter how we split our permutation, there won't be any odd subarrays.</p><p>In the second test case, we can split our permutation into subarrays $[4, 3], [2, 1]$, both of which are odd since their numbers of inversions are $1$.</p><p>In the fourth test case, we can split our permutation into a single subarray $[2, 1]$, which is odd.</p><p>In the fifth test case, we can split our permutation into subarrays $[4, 5], [6, 1, 2, 3]$. The first subarray has $0$ inversions, and the second has $3$, so it is odd.</p>
