## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference between the two versions is the constraint on $n$. You can make hacks only if all versions of the problem are solved.</span></p><p>Let's call an array $a$ of odd length $2m+1$ (with $m \ge 1$) <span class="tex-font-style-bf">bad</span>, if element $a_{m+1}$ is equal to the median of this array. In other words, the array is bad if, after sorting it, the element at $m+1$-st position remains the same.</p><p>Let's call a permutation $p$ of integers from $1$ to $n$ <span class="tex-font-style-bf">anti-median</span>, if every its subarray of odd length $\ge 3$ is not bad.</p><p>You are already given values of some elements of the permutation. Find the number of ways to set unknown values to obtain an <span class="tex-font-style-bf">anti-median</span> permutation. As this number can be very large, find it modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^6)$ &nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, or $p_i = -1$) &nbsp;— the elements of the permutation. If $p_i \neq -1$, it's given, else it's unknown. It's guaranteed that if for some $i \neq j$ holds $p_i \neq -1, p_j \neq -1$, then $p_i \neq p_j$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single integer &nbsp;— the number of ways to set unknown values to obtain an <span class="tex-font-style-bf">anti-median</span> permutation, modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;— the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ $(2 \le n \le 10^6)$ &nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$, or $p_i = -1$) &nbsp;— the elements of the permutation. If $p_i \neq -1$, it's given, else it's unknown. It's guaranteed that if for some $i \neq j$ holds $p_i \neq -1, p_j \neq -1$, then $p_i \neq p_j$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single integer &nbsp;— the number of ways to set unknown values to obtain an <span class="tex-font-style-bf">anti-median</span> permutation, modulo $10^9+7$.</p>





```input1|2,3,6,7,10,11
5
2
-1 -1
3
-1 -1 -1
4
1 2 3 4
6
-1 -1 3 4 -1 -1
8
-1 -1 -1 -1 -1 -1 -1 -1
```




```output1
2
4
0
1
316
```



## Note

<p>In the first test case, both $[1, 2]$ and $[2, 1]$ are anti-median.</p><p>In the second test case, permutations $[1, 3, 2], [2, 1, 3], [2, 3, 1], [3, 1, 2]$ are anti-median. The remaining two permutations, $[1, 2, 3]$, $[3, 2, 1]$, are bad arrays on their own, as their median, $2$, is in their middle.</p><p>In the third test case, $[1, 2, 3, 4]$ isn't anti-median, as it contains bad subarray $[1, 2, 3]$.</p><p>In the fourth test case, the only anti-median array you can get is $[5, 6, 3, 4, 1, 2]$.</p>
