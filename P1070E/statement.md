## Description

<div><p>Polycarp has a lot of work to do. Recently he has learned a new time management rule: "if a task takes five minutes or less, do it immediately". Polycarp likes the new rule, however he is not sure that five minutes is the optimal value. He supposes that this value $d$ should be chosen based on existing task list.</p><p>Polycarp has a list of $n$ tasks to complete. The $i$-th task has difficulty $p_i$, i.e. it requires exactly $p_i$ minutes to be done. Polycarp reads the tasks one by one from the first to the $n$-th. If a task difficulty is $d$ or less, Polycarp starts the work on the task immediately. If a task difficulty is strictly greater than $d$, he will not do the task at all. It is not allowed to rearrange tasks in the list. Polycarp doesn't spend any time for reading a task or skipping it.</p><p>Polycarp has $t$ minutes in total to complete maximum number of tasks. But he does not want to work all the time. He decides to make a break after each group of $m$ consecutive tasks he was working on. The break should take the same amount of time as it was spent in total on completion of these $m$ tasks.</p><p>For example, if $n=7$, $p=[3, 1, 4, 1, 5, 9, 2]$, $d=3$ and $m=2$ Polycarp works by the following schedule:</p><ul> <li> Polycarp reads the first task, its difficulty is not greater than $d$ ($p_1=3 \le d=3$) and works for $3$ minutes (i.e. the minutes $1$, $2$, $3$); </li><li> Polycarp reads the second task, its difficulty is not greater than $d$ ($p_2=1 \le d=3$) and works for $1$ minute (i.e. the minute $4$); </li><li> Polycarp notices that he has finished $m=2$ tasks and takes a break for $3+1=4$ minutes (i.e. on the minutes $5, 6, 7, 8$); </li><li> Polycarp reads the third task, its difficulty is greater than $d$ ($p_3=4 &gt; d=3$) and skips it without spending any time; </li><li> Polycarp reads the fourth task, its difficulty is not greater than $d$ ($p_4=1 \le d=3$) and works for $1$ minute (i.e. the minute $9$); </li><li> Polycarp reads the tasks $5$ and $6$, skips both of them ($p_5&gt;d$ and $p_6&gt;d$); </li><li> Polycarp reads the $7$-th task, its difficulty is not greater than $d$ ($p_7=2 \le d=3$) and works for $2$ minutes (i.e. the minutes $10$, $11$); </li><li> Polycarp notices that he has finished $m=2$ tasks and takes a break for $1+2=3$ minutes (i.e. on the minutes $12, 13, 14$). </li></ul><p>Polycarp stops exactly after $t$ minutes. If Polycarp started a task but has not finished it by that time, the task is not considered as completed. It is allowed to complete less than $m$ tasks in the last group. Also Polycarp considers acceptable to have shorter break than needed after the last group of tasks or even not to have this break at all&nbsp;— his working day is over and he will have enough time to rest anyway.</p><p>Please help Polycarp to find such value $d$, which would allow him to complete maximum possible number of tasks in $t$ minutes.</p></div><div class="input-specification"><p>The first line of the input contains single integer $c$ ($1 \le c \le 5 \cdot 10^4$)&nbsp;— number of test cases. Then description of $c$ test cases follows. Solve test cases separately, test cases are completely independent and do not affect each other.</p><p>Each test case is described by two lines. The first of these lines contains three space-separated integers $n$, $m$ and $t$ ($1 \le n \le 2 \cdot 10^5, 1 \le m \le 2 \cdot 10^5, 1 \le t \le 4 \cdot 10^{10}$)&nbsp;— the number of tasks in Polycarp's list, the number of tasks he can do without a break and the total amount of time Polycarp can work on tasks. The second line of the test case contains $n$ space separated integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le 2 \cdot 10^5$)&nbsp;— difficulties of the tasks.</p><p>The sum of values $n$ for all test cases in the input does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print $c$ lines, each line should contain answer for the corresponding test case&nbsp;— the maximum possible number of tasks Polycarp can complete and the integer value $d$ ($1 \le d \le t$) Polycarp should use in time management rule, separated by space. If there are several possible values $d$ for a test case, output any of them.</p></div>

## Input

<p>The first line of the input contains single integer $c$ ($1 \le c \le 5 \cdot 10^4$)&nbsp;— number of test cases. Then description of $c$ test cases follows. Solve test cases separately, test cases are completely independent and do not affect each other.</p><p>Each test case is described by two lines. The first of these lines contains three space-separated integers $n$, $m$ and $t$ ($1 \le n \le 2 \cdot 10^5, 1 \le m \le 2 \cdot 10^5, 1 \le t \le 4 \cdot 10^{10}$)&nbsp;— the number of tasks in Polycarp's list, the number of tasks he can do without a break and the total amount of time Polycarp can work on tasks. The second line of the test case contains $n$ space separated integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le 2 \cdot 10^5$)&nbsp;— difficulties of the tasks.</p><p>The sum of values $n$ for all test cases in the input does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print $c$ lines, each line should contain answer for the corresponding test case&nbsp;— the maximum possible number of tasks Polycarp can complete and the integer value $d$ ($1 \le d \le t$) Polycarp should use in time management rule, separated by space. If there are several possible values $d$ for a test case, output any of them.</p>





```input1
4
5 2 16
5 6 1 4 7
5 3 30
5 6 1 4 7
6 4 15
12 5 15 7 20 17
1 1 50
100

```




```input2
3
11 1 29
6 4 3 7 5 3 4 7 3 5 3
7 1 5
1 1 1 1 1 1 1
5 2 18
2 3 3 7 5

```




```output1
3 5
4 7
2 10
0 25

```




```output2
4 3
3 1
4 5

```



## Note

<p>In the first test case of the first example $n=5$, $m=2$ and $t=16$. The sequence of difficulties is $[5, 6, 1, 4, 7]$. If Polycarp chooses $d=5$ then he will complete $3$ tasks. Polycarp will work by the following schedule:</p><ul> <li> Polycarp reads the first task, its difficulty is not greater than $d$ ($p_1=5 \le d=5$) and works for $5$ minutes (i.e. the minutes $1, 2, \dots, 5$); </li><li> Polycarp reads the second task, its difficulty is greater than $d$ ($p_2=6 &gt; d=5$) and skips it without spending any time; </li><li> Polycarp reads the third task, its difficulty is not greater than $d$ ($p_3=1 \le d=5$) and works for $1$ minute (i.e. the minute $6$); </li><li> Polycarp notices that he has finished $m=2$ tasks and takes a break for $5+1=6$ minutes (i.e. on the minutes $7, 8, \dots, 12$); </li><li> Polycarp reads the fourth task, its difficulty is not greater than $d$ ($p_4=4 \le d=5$) and works for $4$ minutes (i.e. the minutes $13, 14, 15, 16$); </li><li> Polycarp stops work because of $t=16$. </li></ul><p>In total in the first test case Polycarp will complete $3$ tasks for $d=5$. He can't choose other value for $d$ to increase the number of completed tasks.</p>
