## Description

<div><p>While at Kira's house, Josuke saw a piece of paper on the table with a task written on it.</p><p>The task sounded as follows. There is an array $a$ of length $n$. On this array, do the following:</p><ul> <li> select an integer $k &gt; 1$; </li><li> split the array into $k$ subsegments $^\dagger$; </li><li> calculate the sum in each of $k$ subsegments and write these sums to another array $b$ (where the sum of the subsegment $(l, r)$ is ${\sum_{j = l}^{r}a_j}$); </li><li> the final score of such a split will be $\gcd(b_1, b_2, \ldots, b_k)^\ddagger$. </li></ul><p>The task is to find such a partition that the score is <span class="tex-font-style-bf">maximum possible</span>. Josuke is interested in this task but is not strong in computer science. Help him to find the maximum possible score.</p><p>$^\dagger$ A division of an array into $k$ subsegments is $k$ pairs of numbers $(l_1, r_1), (l_2, r_2), \ldots, (l_k, r_k)$ such that $l_i \le r_i$ and for every $1 \le j \le k - 1$ $l_{j + 1} = r_j + 1$, also $l_1 = 1$ and $r_k = n$. These pairs represent the subsegments.</p><p>$^\ddagger$ $\gcd(b_1, b_2, \ldots, b_k)$ stands for the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of the array $b$.</p></div><div class="input-specification"><p>The first line contains a single number $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>For each test case, the first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, a_3, \ldots, a_n$ ($1 \le a_i \le 10^9 $) — the array $a$ itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print a single integer — the maximum score for the optimal partition.</p></div>

## Input

<p>The first line contains a single number $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>For each test case, the first line contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$) — the length of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, a_3, \ldots, a_n$ ($1 \le a_i \le 10^9 $) — the array $a$ itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print a single integer — the maximum score for the optimal partition.</p>





```input1|2,3,6,7,10,11
6
4
2 2 1 3
2
1 2
3
1 4 5
6
1 2 1 1 1 3
10
12 30 37 88 12 78 89 17 2 12
6
7 7 7 7 7 7
```




```output1
4
1
5
3
1
21
```



## Note

<p>In the first test case, you can choose $k = 2$ and split the array into subsegments $(1, 2)$ and $(3, 4)$.</p><p>Then the score of such a partition will be equal to $\gcd(a_1 + a_2, a_3 + a_4) = \gcd(2 + 2, 1 + 3) = \gcd(4, 4) = 4$.</p><p>In the fourth test case, you can choose $k = 3$ and split the array into subsegments $(1, 2), (3, 5), (6, 6)$.</p><p>The split score is $\gcd(1 + 2, 1 + 1 + 1, 3) = 3$.</p>
