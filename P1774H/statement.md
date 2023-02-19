## Description

<div><p>Ecrade bought a deck of cards numbered from $1$ to $n$. Let the value of a permutation $a$ of length $n$ be $\min\limits_{i = 1}^{n - k + 1}\ \sum\limits_{j = i}^{i + k - 1}a_j$.</p><p>Ecrade wants to find the most valuable one among all permutations of the cards. However, it seems a little difficult, so please help him! </p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 2 \cdot 10^4$) &nbsp;— the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains two integers $n,k$ ($4 \leq k &lt; n \leq 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output the largest possible value in the first line. Then in the second line, print $n$ integers $a_1,a_2,\dots,a_n$ ($1 \le a_i \le n$, all $a_i$ are distinct) &nbsp;— the elements of the permutation that has the largest value.</p><p>If there are multiple such permutations, output any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 2 \cdot 10^4$) &nbsp;— the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains two integers $n,k$ ($4 \leq k &lt; n \leq 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^6$.</p>

## Output

<p>For each test case, output the largest possible value in the first line. Then in the second line, print $n$ integers $a_1,a_2,\dots,a_n$ ($1 \le a_i \le n$, all $a_i$ are distinct) &nbsp;— the elements of the permutation that has the largest value.</p><p>If there are multiple such permutations, output any of them.</p>





```input1|2
2
5 4
8 4
```




```output1
13
1 3 4 5 2 
18
1 8 2 7 3 6 4 5
```



## Note

<p>In the first test case, $[1,4,5,3,2]$ has a value of $13$. It can be shown that no permutations of length $5$ have a value greater than $13$ when $k = 4$.</p><p>In the second test case, $[4,2,5,7,8,3,1,6]$ has a value of $18$. It can be shown that no permutations of length $8$ have a value greater than $18$ when $k = 4$.</p>
