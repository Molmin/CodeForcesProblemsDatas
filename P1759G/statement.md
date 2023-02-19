## Description

<div><p>A sequence of $n$ numbers is called <span class="tex-font-style-it">permutation</span> if it contains all numbers from $1$ to $n$ exactly once. For example, the sequences [$3, 1, 4, 2$], [$1$] and [$2,1$] are permutations, but [$1,2,1$], [$0,1$] and [$1,3,4$]&nbsp;— are not.</p><p>For a permutation $p$ of even length $n$ you can make an array $b$ of length $\frac{n}{2}$ such that: </p><ul> <li> $b_i = \max(p_{2i - 1}, p_{2i})$ for $1 \le i \le \frac{n}{2}$ </li></ul><p>For example, if $p$ = [$2, 4, 3, 1, 5, 6$], then: </p><ul> <li> $b_1 = \max(p_1, p_2) = \max(2, 4) = 4$ </li><li> $b_2 = \max(p_3, p_4) = \max(3,1)=3$ </li><li> $b_3 = \max(p_5, p_6) = \max(5,6) = 6$ </li></ul> As a result, we made $b$ = $[4, 3, 6]$.<p>For a given array $b$, find the <span class="tex-font-style-bf">lexicographically minimal</span> permutation $p$ such that you can make the given array $b$ from it.</p><p>If $b$ = [$4,3,6$], then the lexicographically minimal permutation from which it can be made is $p$ = [$1,4,2,3,5,6$], since: </p><ul> <li> $b_1 = \max(p_1, p_2) = \max(1, 4) = 4$ </li><li> $b_2 = \max(p_3, p_4) = \max(2, 3) = 3$ </li><li> $b_3 = \max(p_5, p_6) = \max(5, 6) = 6$ </li></ul><p>A permutation $x_1, x_2, \dots, x_n$ is lexicographically smaller than a permutation $y_1, y_2 \dots, y_n$ if and only if there exists such $i$ ($1 \le i \le n$) that $x_1=y_1, x_2=y_2, \dots, x_{i-1}=y_{i-1}$ and $x_i&lt;y_i$.</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The description of the test cases follows.</p><p>The first line of each test case contains one even integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains exactly $\frac{n}{2}$ integers $b_i$ ($1 \le b_i \le n$) — elements of array $b$.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print on a separate line: </p><ul> <li> lexicographically minimal permutation $p$ such that you can make an array $b$ from it; </li><li> or a number <span class="tex-font-style-tt">-1</span> if the permutation you are looking for does not exist. </li></ul></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The description of the test cases follows.</p><p>The first line of each test case contains one even integer $n$ ($2 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains exactly $\frac{n}{2}$ integers $b_i$ ($1 \le b_i \le n$) — elements of array $b$.</p><p>It is guaranteed that the sum of $n$ values over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print on a separate line: </p><ul> <li> lexicographically minimal permutation $p$ such that you can make an array $b$ from it; </li><li> or a number <span class="tex-font-style-tt">-1</span> if the permutation you are looking for does not exist. </li></ul>





```input1|2,3,6,7,10,11
6
6
4 3 6
4
2 4
8
8 7 2 3
6
6 4 2
4
4 4
8
8 7 4 5
```




```output1
1 4 2 3 5 6 
1 2 3 4 
-1
5 6 3 4 1 2 
-1
1 8 6 7 2 4 3 5
```



## Note

<p>The first test case is parsed in the problem statement.</p>
