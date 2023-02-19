## Description

<div><p>British mathematician John Littlewood once said about Indian mathematician Srinivasa Ramanujan that "every positive integer was one of his personal friends."</p><p>It turns out that positive integers can also be friends with each other! You are given an array $a$ of distinct positive integers. </p><p>Define a <span class="tex-font-style-bf">subarray</span> $a_i, a_{i+1}, \ldots, a_j$ to be a <span class="tex-font-style-it">friend group</span> if and only if there exists an integer $m \ge 2$ such that $a_i \bmod m = a_{i+1} \bmod m = \ldots = a_j \bmod m$, where $x \bmod y$ denotes the remainder when $x$ is divided by $y$.</p><p>Your friend Gregor wants to know the size of the largest friend group in $a$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2\cdot 10^4$). </p><p>Each test case begins with a line containing the integer $n$ ($1 \le n \le 2 \cdot 10^5$), the size of the array $a$.</p><p>The next line contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le {10}^{18}$), representing the contents of the array $a$. It is guaranteed that all the numbers in $a$ are <span class="tex-font-style-bf">distinct</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases is less than $2\cdot 10^5$.</p></div><div class="output-specification"><p>Your output should consist of $t$ lines. Each line should consist of a single integer, the size of the largest friend group in $a$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2\cdot 10^4$). </p><p>Each test case begins with a line containing the integer $n$ ($1 \le n \le 2 \cdot 10^5$), the size of the array $a$.</p><p>The next line contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le {10}^{18}$), representing the contents of the array $a$. It is guaranteed that all the numbers in $a$ are <span class="tex-font-style-bf">distinct</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases is less than $2\cdot 10^5$.</p>

## Output

<p>Your output should consist of $t$ lines. Each line should consist of a single integer, the size of the largest friend group in $a$.</p>





```input1
4
5
1 5 2 4 6
4
8 2 5 10
2
1000 2000
8
465 55 3 54 234 12 45 78
```




```output1
3
3
2
6
```



## Note

<p>In the first test case, the array is $[1,5,2,4,6]$. The largest friend group is $[2,4,6]$, since all those numbers are congruent to $0$ modulo $2$, so $m=2$.</p><p>In the second test case, the array is $[8,2,5,10]$. The largest friend group is $[8,2,5]$, since all those numbers are congruent to $2$ modulo $3$, so $m=3$.</p><p>In the third case, the largest friend group is $[1000,2000]$. There are clearly many possible values of $m$ that work.</p>
