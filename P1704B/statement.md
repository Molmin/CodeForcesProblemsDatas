## Description

<div><p>Luke likes to eat. There are $n$ piles of food aligned in a straight line in front of him. The $i$-th pile contains $a_i$ units of food. </p><p>Luke will walk from the $1$-st pile towards the $n$-th pile, and he wants to eat every pile of food without walking back. When Luke reaches the $i$-th pile, he can eat that pile if and only if $|v - a_i| \leq x$, where $x$ is a fixed integer, and $v$ is Luke's food affinity.</p><p>Before Luke starts to walk, he can set $v$ to any integer. Also, for each $i$ ($1 \leq i \leq n$), Luke can <span class="tex-font-style-it">change</span> his food affinity to any integer <span class="tex-font-style-bf">before</span> he eats the $i$-th pile.</p><p>Find the minimum number of <span class="tex-font-style-it">changes</span> needed to eat every pile of food.</p><p>Note that the initial choice for $v$ is <span class="tex-font-style-bf">not</span> considered as a change.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of test cases follows.</p><p>For each test case, the first line contains two integers, $n, x$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq x \leq 10^9$) — the number of piles, and the maximum difference between the size of a pile and Luke's food affinity, such that Luke can eat the pile.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots , a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output an integer on a separate line, which is the minimum number of changes needed.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. The description of test cases follows.</p><p>For each test case, the first line contains two integers, $n, x$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq x \leq 10^9$) — the number of piles, and the maximum difference between the size of a pile and Luke's food affinity, such that Luke can eat the pile.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots , a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output an integer on a separate line, which is the minimum number of changes needed.</p>





```input1|2,3,6,7,10,11,14,15
7
5 3
3 8 5 6 7
5 3
3 10 9 8 7
12 8
25 3 3 17 8 6 1 16 15 25 17 23
10 2
1 2 3 4 5 6 7 8 9 10
8 2
2 4 6 8 6 4 12 14
8 2
2 7 8 9 6 13 21 28
15 5
11 4 13 23 7 10 5 21 20 11 17 5 29 16 11
```




```output1
0
1
2
1
2
4
6
```



## Note

<p>In the first test case, Luke can set $v$ to $5$ before he starts to walk. And he can walk straight to eat every piles of food without changing $v$.</p><p>In the second test case, Luke can set $v$ to $3$ before he starts to walk. And he could change $v$ to $10$ before he eats the second pile. After that, he can walk straight to eat remaining food without changing $v$.</p><p>In the fourth test case, Luke can set $v$ to $3$ before he starts to walk. And he could change $v$ to $8$ before he eats the sixth pile. After that, he can walk straight to eat remaining food without changing $v$.</p><p>In the fifth test case, Luke can set $v$ to $4$ before he starts to walk. And he could change $v$ to $6$ before he eats the fourth pile. Then he could change $v$ to $12$ before he eats the seventh pile. After that, he can walk straight to eat remaining food without changing $v$.</p>
