## Description

<div><p>You are given a set $a_1, a_2, \ldots, a_n$ of distinct positive integers.</p><p>We define the <span class="tex-font-style-it">squareness</span> of an integer $x$ as the number of perfect squares among the numbers $a_1 + x, a_2 + x, \ldots, a_n + x$.</p><p>Find the maximum squareness among all integers $x$ between $0$ and $10^{18}$, inclusive.</p><p>Perfect squares are integers of the form $t^2$, where $t$ is a non-negative integer. The smallest perfect squares are $0, 1, 4, 9, 16, \ldots$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 50$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;($1 \le n \le 50$)&nbsp;— the size of the set.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ in increasing order&nbsp;($1 \le a_1 &lt; a_2 &lt; \ldots &lt; a_n \le 10^9$)&nbsp;— the set itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $50$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the largest possible number of perfect squares among $a_1 + x, a_2 + x, \ldots, a_n + x$, for some $0 \le x \le 10^{18}$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 50$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;($1 \le n \le 50$)&nbsp;— the size of the set.</p><p>The second line contains $n$ distinct integers $a_1, a_2, \ldots, a_n$ in increasing order&nbsp;($1 \le a_1 &lt; a_2 &lt; \ldots &lt; a_n \le 10^9$)&nbsp;— the set itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $50$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the largest possible number of perfect squares among $a_1 + x, a_2 + x, \ldots, a_n + x$, for some $0 \le x \le 10^{18}$.</p>





```input1|2,3,6,7
4
5
1 2 3 4 5
5
1 6 13 22 97
1
100
5
2 5 10 17 26
```




```output1
2
5
1
2
```



## Note

<p>In the first test case, for $x = 0$ the set contains two perfect squares: $1$ and $4$. It is impossible to obtain more than two perfect squares.</p><p>In the second test case, for $x = 3$ the set looks like $4, 9, 16, 25, 100$, that is, all its elements are perfect squares.</p>
