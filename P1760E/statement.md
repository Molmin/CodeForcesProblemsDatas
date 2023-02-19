## Description

<div><p>You are given a binary array$^{\dagger}$ of length $n$. You are allowed to perform one operation on it <span class="tex-font-style-bf">at most once</span>. In an operation, you can choose any element and flip it: turn a $0$ into a $1$ or vice-versa.</p><p>What is the maximum number of inversions$^{\ddagger}$ the array can have after performing <span class="tex-font-style-bf">at most one</span> operation?</p><p>$^\dagger$ A binary array is an array that contains only zeroes and ones.</p><p>$^\ddagger$ The number of inversions in an array is the number of pairs of indices $i,j$ such that $i&lt;j$ and $a_i &gt; a_j$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated positive integers $a_1$, $a_2$,..., $a_n$ ($0 \leq a_i \leq 1$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the maximum number of inversions the array can have after performing <span class="tex-font-style-bf">at most one</span> operation.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated positive integers $a_1$, $a_2$,..., $a_n$ ($0 \leq a_i \leq 1$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the maximum number of inversions the array can have after performing <span class="tex-font-style-bf">at most one</span> operation.</p>





```input1|2,3,6,7,10,11
5
4
1 0 1 0
6
0 1 0 0 1 0
2
0 0
8
1 0 1 1 0 0 0 1
3
1 1 1
```




```output1
3
7
1
13
2
```



## Note

<p>For the first test case, the inversions are initially formed by the pairs of indices ($1, 2$), ($1, 4$), ($3, 4$), being a total of $3$, which already is the maximum possible.</p><p>For the second test case, the inversions are initially formed by the pairs of indices ($2, 3$), ($2, 4$), ($2, 6$), ($5, 6$), being a total of four. But, by flipping the first element, the array becomes ${1, 1, 0, 0, 1, 0}$, which has the inversions formed by the pairs of indices ($1, 3$), ($1, 4$), ($1, 6$), ($2, 3$), ($2, 4$), ($2, 6$), ($5, 6$) which total to $7$ inversions which is the maximum possible.</p>
