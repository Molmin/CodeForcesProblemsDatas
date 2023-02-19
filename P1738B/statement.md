## Description

<div><p>Suppose $a_1, a_2, \dots, a_n$ is a sorted <span class="tex-font-style-bf">integer</span> sequence of length $n$ such that $a_1 \leq a_2 \leq \dots \leq a_n$. </p><p>For every $1 \leq i \leq n$, the prefix sum $s_i$ of the first $i$ terms $a_1, a_2, \dots, a_i$ is defined by $$ s_i = \sum_{k=1}^i a_k = a_1 + a_2 + \dots + a_i. $$</p><p>Now you are given the last $k$ terms of the prefix sums, which are $s_{n-k+1}, \dots, s_{n-1}, s_{n}$. Your task is to determine whether this is possible. </p><p>Formally, given $k$ integers $s_{n-k+1}, \dots, s_{n-1}, s_{n}$, the task is to check whether there is a sequence $a_1, a_2, \dots, a_n$ such that </p><ol> <li> $a_1 \leq a_2 \leq \dots \leq a_n$, and </li><li> $s_i = a_1 + a_2 + \dots + a_i$ for all $n-k+1 \leq i \leq n$. </li></ol></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains two integers $n$ ($1 \leq n \leq 10^5$) and $k$ ($1 \leq k \leq n$), indicating the length of the sequence $a$ and the number of terms of prefix sums, respectively.</p><p>The second line of each test case contains $k$ integers $s_{n-k+1}, \dots, s_{n-1}, s_{n}$ ($-10^9 \leq s_i \leq 10^9$ for every $n-k+1 \leq i \leq n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 10^5$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains two integers $n$ ($1 \leq n \leq 10^5$) and $k$ ($1 \leq k \leq n$), indicating the length of the sequence $a$ and the number of terms of prefix sums, respectively.</p><p>The second line of each test case contains $k$ integers $s_{n-k+1}, \dots, s_{n-1}, s_{n}$ ($-10^9 \leq s_i \leq 10^9$ for every $n-k+1 \leq i \leq n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output "<span class="tex-font-style-tt">YES</span>" and "<span class="tex-font-style-tt">NO</span>" in any case (for example, strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>" and "<span class="tex-font-style-tt">Yes</span>" will be recognized as a positive response).</p>





```input1|2,3,6,7
4
5 5
1 2 3 4 5
7 4
-6 -5 -3 0
3 3
2 3 4
3 2
3 4
```




```output1
Yes
Yes
No
No
```



## Note

<p>In the first test case, we have the only sequence $a = [1, 1, 1, 1, 1]$.</p><p>In the second test case, we can choose, for example, $a = [-3, -2, -1, 0, 1, 2, 3]$.</p><p>In the third test case, the prefix sums define the only sequence $a = [2, 1, 1]$, but it is not sorted. </p><p>In the fourth test case, it can be shown that there is no sequence with the given prefix sums.</p>
