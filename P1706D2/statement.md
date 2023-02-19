## Description

<div><p><span class="tex-font-style-it">This is the hard version of the problem. The only difference between the versions is the constraints on $n$, $k$, $a_i$, and the sum of $n$ over all test cases. You can make hacks only if both versions of the problem are solved.</span></p><p><span class="tex-font-style-bf">Note the unusual memory limit.</span></p><p>You are given an array of integers $a_1, a_2, \ldots, a_n$ of length $n$, and an integer $k$.</p><p>The <span class="tex-font-style-it">cost</span> of an array of integers $p_1, p_2, \ldots, p_n$ of length $n$ is $$\max\limits_{1 \le i \le n}\left(\left \lfloor \frac{a_i}{p_i} \right \rfloor \right) - \min\limits_{1 \le i \le n}\left(\left \lfloor \frac{a_i}{p_i} \right \rfloor \right).$$</p><p>Here, $\lfloor \frac{x}{y} \rfloor$ denotes the integer part of the division of $x$ by $y$. Find the minimum cost of an array $p$ such that $1 \le p_i \le k$ for all $1 \le i \le n$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n, k \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_1 \le a_2 \le \ldots \le a_n \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the minimum possible cost of an array $p$ satisfying the condition above.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n, k \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_1 \le a_2 \le \ldots \le a_n \le 10^5$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the minimum possible cost of an array $p$ satisfying the condition above.</p>





```input1|2,3,6,7,10,11,14,15
7
5 2
4 5 6 8 11
5 12
4 5 6 8 11
3 1
2 9 15
7 3
2 3 5 5 6 9 10
6 56
54 286 527 1436 2450 2681
3 95
16 340 2241
2 2
1 3
```




```output1
2
0
13
1
4
7
0
```



## Note

<p>In the first test case, the optimal array is $p = [1, 1, 1, 2, 2]$. The resulting array of values of $\lfloor \frac{a_i}{p_i} \rfloor$ is $[4, 5, 6, 4, 5]$. The cost of $p$ is $\max\limits_{1 \le i \le n}(\lfloor \frac{a_i}{p_i} \rfloor) - \min\limits_{1 \le i \le n}(\lfloor \frac{a_i}{p_i} \rfloor) = 6 - 4 = 2$. We can show that there is no array (satisfying the condition from the statement) with a smaller cost.</p><p>In the second test case, one of the optimal arrays is $p = [12, 12, 12, 12, 12]$, which results in all $\lfloor \frac{a_i}{p_i} \rfloor$ being $0$.</p><p>In the third test case, the only possible array is $p = [1, 1, 1]$.</p>
