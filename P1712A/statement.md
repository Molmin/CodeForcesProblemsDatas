## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">God's Blessing on This PermutationForces!</span></div><div class="epigraph-source">A Random Pebble</div></div><p>You are given a permutation $p_1,p_2,\ldots,p_n$ of length $n$ and a positive integer $k \le n$. </p><p>In one operation you can choose two indices $i$ and $j$ ($1 \le i &lt; j \le n$) and swap $p_i$ with $p_j$.</p><p>Find the minimum number of operations needed to make the sum $p_1 + p_2 + \ldots + p_k$ as small as possible.</p><p>A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 100$).</p><p>The second line of each test case contains $n$ integers $p_1,p_2,\ldots,p_n$ ($1 \le p_i \le n$). It is guaranteed that the given numbers form a permutation of length $n$.</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the minimum number of operations needed to make the sum $p_1 + p_2 + \ldots + p_k$ as small as possible.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le k \le n \le 100$).</p><p>The second line of each test case contains $n$ integers $p_1,p_2,\ldots,p_n$ ($1 \le p_i \le n$). It is guaranteed that the given numbers form a permutation of length $n$.</p>

## Output

<p>For each test case print one integer&nbsp;— the minimum number of operations needed to make the sum $p_1 + p_2 + \ldots + p_k$ as small as possible.</p>





```input1|2,3,6,7
4
3 1
2 3 1
3 3
1 2 3
4 2
3 4 1 2
1 1
1
```




```output1
1
0
2
0
```



## Note

<p>In the first test case, the value of $p_1 + p_2 + \ldots + p_k$ is initially equal to $2$, but the smallest possible value is $1$. You can achieve it by swapping $p_1$ with $p_3$, resulting in the permutation $[1, 3, 2]$.</p><p>In the second test case, the sum is already as small as possible, so the answer is $0$.</p>
