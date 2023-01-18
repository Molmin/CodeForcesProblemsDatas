## Description

<div><p>For the first time, Polycarp's startup ended the year with a profit! Now he is about to distribute $k$ burles as a bonus among $n$ employees.</p><p>It is known that the current salary of the $i$-th employee is $a_i$ and all the values of $a_i$ in the company are <span class="tex-font-style-bf">different</span>.</p><p>Polycarp wants to distribute the $k$ burles between $n$ employees so this month the $i$-th employee will be paid not $a_i$, but $a_i+d_i$ ($d_i \ge 0$, $d_i$ is an integer), where $d_i$ is the bonus for the $i$-th employee. Of course, $d_1+d_2+\dots+d_n=k$.</p><p>Polycarp will follow two rules for choosing the values $d_i$:</p><ul> <li> the relative order of the salaries should not be changed: the employee with originally the highest salary ($a_i$ is the maximum) should have the highest total payment after receiving their bonus ($a_i+d_i$ is also the maximum), the employee whose salary was originally the second-largest should receive the second-largest total payment after receiving their bonus and so on. </li><li> to emphasize that annual profit is a group effort, Polycarp wants to <span class="tex-font-style-bf">minimize</span> the maximum total payment to an employee (i.e minimize the maximum value of $a_i+d_i$). </li></ul><p>Help Polycarp decide the non-negative integer bonuses $d_i$ such that:</p><ul> <li> their sum is $k$, </li><li> for each employee, the number of those who receive <span class="tex-font-style-bf">strictly more</span> than them remains unchanged (that is, if you sort employees by $a_i$ and by $a_i+d_i$, you get the same order of employees), </li><li> all $a_i + d_i$ are different, </li><li> the maximum of the values $a_i+d_i$ is the minimum possible. </li></ul><p>Help Polycarp and print any of the possible answers $d_1, d_2, \dots, d_n$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $1 \le k \le 10^9$)&nbsp;— the number of employees and the total bonus.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">different</span> integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the current salary of the $i$-th employee.</p><p>It is guaranteed that the sum of all $n$ values in the input does not exceed $10^5$.</p></div><div class="output-specification"><p>Print the answers to $t$ test cases in the order they appear in the input. Print each answer as a sequence of non-negative integers $d_1, d_2, \dots, d_n$. If there are several answers, print any of them.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 10^5$, $1 \le k \le 10^9$)&nbsp;— the number of employees and the total bonus.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">different</span> integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the current salary of the $i$-th employee.</p><p>It is guaranteed that the sum of all $n$ values in the input does not exceed $10^5$.</p>

## Output

<p>Print the answers to $t$ test cases in the order they appear in the input. Print each answer as a sequence of non-negative integers $d_1, d_2, \dots, d_n$. If there are several answers, print any of them.</p>





```input1
5
4 1
3 1 4 2
2 3
10 2
4 1000000000
987654321 1000000000 999999999 500000000
8 9
5 6 1 8 3 4 2 7
6 1
6 3 1 8 5 9
```




```output1
0 0 1 0 
0 3 
134259259 121913582 121913582 621913577 
2 2 0 2 0 1 0 2 
1 0 0 0 0 0
```


