## Description

<div><p>Vitaly enrolled in the course Advanced Useless Algorithms. The course consists of $n$ tasks. Vitaly calculated that he has $a_i$ hours to do the task $i$ from the day he enrolled in the course. That is, the deadline before the $i$-th task is $a_i$ hours. The array $a$ is sorted in ascending order, in other words, the job numbers correspond to the order in which the assignments are turned in.</p><p>Vitaly does everything conscientiously, so he wants to complete <span class="tex-font-style-bf">each</span> task by $100$ percent, <span class="tex-font-style-bf">or more</span>. Initially, his completion rate for each task is $0$ percent.</p><p>Vitaly has $m$ training options, each option can be used <span class="tex-font-style-bf">not more than</span> once. The $i$th option is characterized by three integers: $e_i, t_i$ and $p_i$. If Vitaly uses the $i$th option, then after $t_i$ hours (from the current moment) he will increase the progress of the task $e_i$ by $p_i$ percent. </p><p>For example, let Vitaly have $3$ of tasks to complete. Let the array $a$ have the form: $a = [5, 7, 8]$. Suppose Vitaly has $5$ of options: $[e_1=1, t_1=1, p_1=30]$, $[e_2=2, t_2=3, p_2=50]$, $[e_3=2, t_3=3, p_3=100]$, $[e_4=1, t_4=1, p_4=80]$, $[e_5=3, t_5=3, p_5=100]$. </p><p>Then, if Vitaly prepares in the following way, he will be able to complete everything in time: </p><ul> <li> Vitaly chooses the $4$-th option. Then in $1$ hour, he will complete the $1$-st task at $80$ percent. He still has $4$ hours left before the deadline for the $1$-st task. </li><li> Vitaly chooses the $3$-rd option. Then in $3$ hours, he will complete the $2$-nd task in its entirety. He has another $1$ hour left before the deadline for the $1$-st task and $4$ hours left before the deadline for the $3$-rd task. </li><li> Vitaly chooses the $1$-st option. Then after $1$ hour, he will complete the $1$-st task for $110$ percent, which means that he will complete the $1$-st task just in time for the deadline. </li><li> Vitaly chooses the $5$-th option. He will complete the $3$-rd task for $2$ hours, and after another $1$ hour, Vitaly will complete the $3$-rd task in its entirety. </li></ul><p>Thus, Vitaly has managed to complete the course completely and on time, using the $4$ options.</p><p>Help Vitaly&nbsp;— print the options for Vitaly to complete the tasks in the correct order. Please note: each option can be used <span class="tex-font-style-bf">not more than</span> once. If there are several possible answers, it is allowed to output any of them.</p></div><div class="input-specification"><p>The first line of input data contains an integer $T$ ($1 \le T \le 10^4$)&nbsp;—the number of input test cases in the test.</p><p>The descriptions of the input test case follow.</p><p>The first line of each test case description contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$)&nbsp;—the number of jobs and the number of training options, respectively.</p><p>The next line contains $n$ numbers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the time before the deadline of job $i$. The array values&nbsp;— are non-decreasing, that is $a_1 \le a_2 \le \dots \le a_n$.</p><p>The following $m$ lines contain triples of numbers $e_i, t_i, p_i$ ($1 \le e_i \le n$, $1 \le t_i \le 10^9$, $1 \le p_i \le 100$)&nbsp;— if Vitaly chooses this option, then after $t_i$ hours he will increase the progress of the task $e_i$ by $p_i$ percent. The options are numbered from $1$ to $m$ in order in the input data.</p><p>It is guaranteed that the sum of $n+m$ on all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print on the first line the number $k$, meaning that for $k$ of options, Vitaly will be able to complete each task by $100$ percent or more on time. The options should not be repeated. Or print <span class="tex-font-style-tt">-1</span> if Vitaly is unable to complete all tasks in time.</p><p>If there is an answer, on the next line print $k$ of different integers from $1$ to $m$&nbsp;— the numbers of the options in the order you want. If there is more than one answer, it is allowed to print <span class="tex-font-style-bf">any</span> of them.</p></div>

## Input

<p>The first line of input data contains an integer $T$ ($1 \le T \le 10^4$)&nbsp;—the number of input test cases in the test.</p><p>The descriptions of the input test case follow.</p><p>The first line of each test case description contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$)&nbsp;—the number of jobs and the number of training options, respectively.</p><p>The next line contains $n$ numbers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the time before the deadline of job $i$. The array values&nbsp;— are non-decreasing, that is $a_1 \le a_2 \le \dots \le a_n$.</p><p>The following $m$ lines contain triples of numbers $e_i, t_i, p_i$ ($1 \le e_i \le n$, $1 \le t_i \le 10^9$, $1 \le p_i \le 100$)&nbsp;— if Vitaly chooses this option, then after $t_i$ hours he will increase the progress of the task $e_i$ by $p_i$ percent. The options are numbered from $1$ to $m$ in order in the input data.</p><p>It is guaranteed that the sum of $n+m$ on all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print on the first line the number $k$, meaning that for $k$ of options, Vitaly will be able to complete each task by $100$ percent or more on time. The options should not be repeated. Or print <span class="tex-font-style-tt">-1</span> if Vitaly is unable to complete all tasks in time.</p><p>If there is an answer, on the next line print $k$ of different integers from $1$ to $m$&nbsp;— the numbers of the options in the order you want. If there is more than one answer, it is allowed to print <span class="tex-font-style-bf">any</span> of them.</p>





```input1|2,3,4,5,6,7,8,16,17,18,19,20,21,22,23,24,25,26,31,32,33,34,35,36,37
5
3 5
5 7 8
1 1 30
2 3 50
2 3 100
1 1 80
3 3 100
1 5
51
1 36 91
1 8 40
1 42 83
1 3 45
1 13 40
2 9
9 20
2 8 64
2 7 64
1 20 56
2 8 76
2 20 48
1 2 89
1 3 38
2 18 66
1 7 51
3 2
7 18 33
1 5 80
3 4 37
2 5
569452312 703565975
1 928391659 66
1 915310 82
2 87017081 92
1 415310 54
2 567745964 82
```




```input2|2,3,4,5,6,7,8,9,10,11,12,21,22,23
3
3 9
20 31 40
1 9 64
3 17 100
3 9 59
3 18 57
3 20 49
2 20 82
2 14 95
1 8 75
2 16 67
2 6
20 36
2 2 66
2 20 93
1 3 46
1 10 64
2 8 49
2 18 40
1 1
1000000000
1 1000000000 100
```




```output1
4
1 4 3 5 
3
2 4 5 
4
6 7 1 2 
-1
4
2 4 3 5
```




```output2
-1
4
3 4 1 5 
1
1
```


