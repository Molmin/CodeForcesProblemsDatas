## Description

<div><p>You are given a permutation $p_1, p_2, \ldots, p_n$ of length $n$ of numbers $0, \ldots, n - 1$. Count the number of subsegments $1 \leq l \leq r \leq n$ of this permutation such that $mex(p_l, p_{l+1}, \ldots, p_r) &gt; med(p_l, p_{l+1}, \ldots, p_r)$.</p><p>$mex$ of $S$ is the smallest non-negative integer that does not occur in $S$. For example:</p><ul><li> $mex({0, 1, 2, 3}) = 4$</li><li> $mex({0, 4, 1, 3}) = 2$</li><li> $mex({5, 4, 0, 1, 2}) = 3$</li></ul><p>$med$ of the set $S$ is the median of the set, i.e. the element that, after sorting the elements in non-decreasing order, will be at position number $\left \lfloor{ \frac{|S| + 1}{2} } \right \rfloor$ (array elements are numbered starting from $1$ and here $\left \lfloor{v} \right \rfloor$ denotes rounding $v$ down.). For example:</p><ul><li> $med({0, 1, 2, 3}) = 1$</li><li> $med({0, 4, 1, 3}) = 1$</li><li> $med({5, 4, 0, 1, 2}) = 2$</li></ul><p>A sequence of $n$ numbers is called a permutation if it contains all the numbers from $0$ to $n - 1$ exactly once.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10^4$), the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$), the length of the permutation $p$.</p><p>The second line of each test case contains exactly $n$ integers: $p_1, p_2, \ldots, p_n$ ($0 \leq p_i \leq n - 1$), elements of permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print the answer in a single line: the number of subsegments $1 \leq l \leq r \leq n$ of this permutation such that $mex(p_l, p_{l+1}, \ldots, p_r) &gt; med(p_l, p_{l+1}, \ldots, p_r)$.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10^4$), the number of test cases.</p><p>The descriptions of the test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2 \cdot 10^5$), the length of the permutation $p$.</p><p>The second line of each test case contains exactly $n$ integers: $p_1, p_2, \ldots, p_n$ ($0 \leq p_i \leq n - 1$), elements of permutation $p$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print the answer in a single line: the number of subsegments $1 \leq l \leq r \leq n$ of this permutation such that $mex(p_l, p_{l+1}, \ldots, p_r) &gt; med(p_l, p_{l+1}, \ldots, p_r)$.</p>





```input1|2,3,6,7,10,11,14,15
8
1
0
2
1 0
3
1 0 2
4
0 2 1 3
5
3 1 0 2 4
6
2 0 4 1 3 5
8
3 7 2 6 0 1 5 4
4
2 0 1 3
```




```output1
1
2
4
4
8
8
15
6
```



## Note

<p>The first test case contains exactly one subsegment and $mex({0}) = 1 &gt; med({0}) = 0$ on it.</p><p>In the third test case, on the following subsegments: $[1, 0]$, $[0]$, $[1, 0, 2]$ and $[0, 2]$, $mex$ is greater than $med$.</p><p>In the fourth test case, on the following subsegments: $[0, 2]$, $[0]$, $[0, 2, 1]$ and $[0, 2, 1, 3]$, $mex$ greater than $med$.</p>
