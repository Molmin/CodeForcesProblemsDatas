## Description

<div><p>There is a street that can be represented as an array of length $n$.</p><p>There are two policemen patrolling a street: the first one is standing at the point $x$ of the street and the second one is standing at the point $y$ of the street.</p><p>During one minute, both policemen can decide what to do (independently): move left (if the current position is greater than $1$), move right (if the current position is less than $n$), or do nothing.</p><p>The street is considered clear if <span class="tex-font-style-bf">each</span> point of the street is visited by at least one policeman.</p><p>Your task is to find the minimum number of minutes the policemen need to visit <span class="tex-font-style-bf">each</span> point of the street (again, each point should be visited by at least one of them).</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains three integers $n$, $x$ and $y$ ($2 \le n \le 10^6$; $1 \le x, y \le n$; $x \ne y$) — the length of the street, the position of the first policeman and the position of the second policeman, respectively.</p><p>It is guaranteed that the sum of $n$ does not exceed $10^6$ ($\sum n \le 10^6$).</p></div><div class="output-specification"><p>For each test case, print one integer — the minimum number of minutes the policemen need to visit <span class="tex-font-style-bf">each</span> point of the street.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains three integers $n$, $x$ and $y$ ($2 \le n \le 10^6$; $1 \le x, y \le n$; $x \ne y$) — the length of the street, the position of the first policeman and the position of the second policeman, respectively.</p><p>It is guaranteed that the sum of $n$ does not exceed $10^6$ ($\sum n \le 10^6$).</p>

## Output

<p>For each test case, print one integer — the minimum number of minutes the policemen need to visit <span class="tex-font-style-bf">each</span> point of the street.</p>





```input1
6
4 1 2
7 7 1
10 2 6
8 5 2
2 1 2
20 4 14
```




```output1
2
3
5
4
0
12
```


