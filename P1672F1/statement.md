## Description

<div><p>oolimry has an array $a$ of length $n$ which he really likes. Today, you have changed his array to $b$, a permutation of $a$, to make him sad.</p><p>Because oolimry is only a duck, he can only perform the following operation to restore his array: </p><ul> <li> Choose two integers $i,j$ such that $1 \leq i,j \leq n$. </li><li> Swap $b_i$ and $b_j$. </li></ul><p>The <span class="tex-font-style-bf">sadness</span> of the array $b$ is the minimum number of operations needed to transform $b$ into $a$.</p><p>Given the array $a$, find any array $b$ which is a permutation of $a$ that has the maximum sadness over all permutations of the array $a$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) &nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$) &nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $n$ integers $b_1, b_2, \ldots, b_n$ — describing the array $b$. If there are multiple answers, you may print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) &nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq n$) &nbsp;— elements of the array $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $n$ integers $b_1, b_2, \ldots, b_n$ — describing the array $b$. If there are multiple answers, you may print any.</p>





```input1
2
2
2 1
4
1 2 3 3
```




```output1
1 2
3 3 2 1
```



## Note

<p>In the first test case, the array $[1,2]$ has sadness $1$. We can transform $[1,2]$ into $[2,1]$ using one operation with $(i,j)=(1,2)$.</p><p>In the second test case, the array $[3,3,2,1]$ has sadness $2$. We can transform $[3,3,2,1]$ into $[1,2,3,3]$ with two operations with $(i,j)=(1,4)$ and $(i,j)=(2,3)$ respectively.</p>
