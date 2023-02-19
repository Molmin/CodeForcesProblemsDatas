## Description

<div><p>For his birthday, Kevin received the set of pairwise distinct numbers $1, 2, 3, \ldots, n$ as a gift.</p><p>He is going to arrange these numbers in a way such that the minimum absolute difference between two consecutive numbers be maximum possible. More formally, if he arranges numbers in order $p_1, p_2, \ldots, p_n$, he wants to maximize the value $$\min \limits_{i=1}^{n - 1} \lvert p_{i + 1} - p_i \rvert,$$ where $|x|$ denotes the absolute value of $x$.</p><p>Help Kevin to do that.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains an integer $n$ ($2 \le n \leq 1\,000$)&nbsp;— the size of the set.</p></div><div class="output-specification"><p>For each test case print a single line containing $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$) describing the arrangement that maximizes the minimum absolute difference of consecutive elements. </p><p>Formally, you have to print a permutation $p$ which maximizes the value $\min \limits_{i=1}^{n - 1} \lvert p_{i + 1} - p_i \rvert$.</p><p>If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The only line of each test case contains an integer $n$ ($2 \le n \leq 1\,000$)&nbsp;— the size of the set.</p>

## Output

<p>For each test case print a single line containing $n$ distinct integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$) describing the arrangement that maximizes the minimum absolute difference of consecutive elements. </p><p>Formally, you have to print a permutation $p$ which maximizes the value $\min \limits_{i=1}^{n - 1} \lvert p_{i + 1} - p_i \rvert$.</p><p>If there are multiple optimal solutions, print any of them.</p>





```input1|2
2
4
3
```




```output1
2 4 1 3
1 2 3
```



## Note

<p>In the first test case the minimum absolute difference of consecutive elements equals $\min \{\lvert 4 - 2 \rvert, \lvert 1 - 4 \rvert, \lvert 3 - 1 \rvert \} = \min \{2, 3, 2\} = 2$. It's easy to prove that this answer is optimal.</p><p>In the second test case each permutation of numbers $1, 2, 3$ is an optimal answer. The minimum absolute difference of consecutive elements equals to $1$.</p>
