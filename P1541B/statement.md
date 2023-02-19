## Description

<div><p>You are given an array $a_1, a_2, \dots, a_n$ consisting of $n$ <span class="tex-font-style-bf">distinct</span> integers. Count the number of pairs of indices $(i, j)$ such that $i &lt; j$ and $a_i \cdot a_j = i + j$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ space separated integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 2 \cdot n$)&nbsp;— the array $a$. It is guaranteed that all elements are <span class="tex-font-style-bf">distinct</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the number of pairs of indices $(i, j)$ such that $i &lt; j$ and $a_i \cdot a_j = i + j$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 10^5$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ space separated integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 2 \cdot n$)&nbsp;— the array $a$. It is guaranteed that all elements are <span class="tex-font-style-bf">distinct</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output the number of pairs of indices $(i, j)$ such that $i &lt; j$ and $a_i \cdot a_j = i + j$.</p>





```input1
3
2
3 1
3
6 1 5
5
3 1 5 9 2
```




```output1
1
1
3
```



## Note

<p>For the first test case, the only pair that satisfies the constraints is $(1, 2)$, as $a_1 \cdot a_2 = 1 + 2 = 3$</p><p>For the second test case, the only pair that satisfies the constraints is $(2, 3)$.</p><p>For the third test case, the pairs that satisfy the constraints are $(1, 2)$, $(1, 5)$, and $(2, 3)$.</p>
