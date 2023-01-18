## Description

<div><p>$n$ students are taking an exam. The highest possible score at this exam is $m$. Let $a_{i}$ be the score of the $i$-th student. You have access to the school database which stores the results of all students.</p><p>You can change each student's score as long as the following conditions are satisfied: </p><ul> <li> All scores are integers </li><li> $0 \leq a_{i} \leq m$ </li><li> The average score of the class doesn't change. </li></ul><p>You are student $1$ and you would like to maximize your own score.</p><p>Find the highest possible score you can assign to yourself such that all conditions are satisfied.</p></div><div class="input-specification"><p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 200$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n \leq 10^{3}$, $1 \leq m \leq 10^{5}$) &nbsp;— the number of students and the highest possible score respectively.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($ 0 \leq a_{i} \leq m$) &nbsp;— scores of the students.</p></div><div class="output-specification"><p>For each testcase, output one integer &nbsp;— the highest possible score you can assign to yourself such that both conditions are satisfied._</p></div>

## Input

<p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 200$). The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n \leq 10^{3}$, $1 \leq m \leq 10^{5}$) &nbsp;— the number of students and the highest possible score respectively.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($ 0 \leq a_{i} \leq m$) &nbsp;— scores of the students.</p>

## Output

<p>For each testcase, output one integer &nbsp;— the highest possible score you can assign to yourself such that both conditions are satisfied._</p>





```input1
2
4 10
1 2 3 4
4 5
1 2 3 4
```




```output1
10
5
```



## Note

<p>In the first case, $a = [1,2,3,4] $, with average of $2.5$. You can change array $a$ to $[10,0,0,0]$. Average remains $2.5$, and all conditions are satisfied.</p><p>In the second case, $0 \leq a_{i} \leq 5$. You can change $a$ to $[5,1,1,3]$. You cannot increase $a_{1}$ further as it will violate condition $0\le a_i\le m$.</p>
