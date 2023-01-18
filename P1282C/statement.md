## Description

<div><p>Petya has come to the math exam and wants to solve as many problems as possible. He prepared and carefully studied the rules by which the exam passes.</p><p>The exam consists of $n$ problems that can be solved in $T$ minutes. Thus, the exam begins at time $0$ and ends at time $T$. Petya can leave the exam at any integer time from $0$ to $T$, inclusive.</p><p>All problems are divided into two types: </p><ul> <li> easy problems — Petya takes exactly $a$ minutes to solve any easy problem; </li><li> hard problems — Petya takes exactly $b$ minutes ($b &gt; a$) to solve any hard problem. </li></ul><p>Thus, if Petya starts solving an easy problem at time $x$, then it will be solved at time $x+a$. Similarly, if at a time $x$ Petya starts to solve a hard problem, then it will be solved at time $x+b$.</p><p>For every problem, Petya knows if it is easy or hard. Also, for each problem is determined time $t_i$ ($0 \le t_i \le T$) at which it will become <span class="tex-font-style-it">mandatory</span> (required). If Petya leaves the exam at time $s$ and there is such a problem $i$ that $t_i \le s$ and he didn't solve it, then he will receive $0$ points for the whole exam. Otherwise (i.e if he has solved all such problems for which $t_i \le s$) he will receive a number of points equal to the number of solved problems. Note that leaving at time $s$ Petya can have both "mandatory" and "non-mandatory" problems solved.</p><p>For example, if $n=2$, $T=5$, $a=2$, $b=3$, the first problem is hard and $t_1=3$ and the second problem is easy and $t_2=2$. Then:</p><ul> <li> if he leaves at time $s=0$, then he will receive $0$ points since he will not have time to solve any problems; </li><li> if he leaves at time $s=1$, he will receive $0$ points since he will not have time to solve any problems; </li><li> if he leaves at time $s=2$, then he can get a $1$ point by solving the problem with the number $2$ (it must be solved in the range from $0$ to $2$); </li><li> if he leaves at time $s=3$, then he will receive $0$ points since at this moment both problems will be mandatory, but he will not be able to solve both of them; </li><li> if he leaves at time $s=4$, then he will receive $0$ points since at this moment both problems will be mandatory, but he will not be able to solve both of them; </li><li> if he leaves at time $s=5$, then he can get $2$ points by solving all problems. </li></ul><p>Thus, the answer to this test is $2$.</p><p>Help Petya to determine the maximal number of points that he can receive, before leaving the exam.</p></div><div class="input-specification"><p>The first line contains the integer $m$ ($1 \le m \le 10^4$)&nbsp;— the number of test cases in the test.</p><p>The next lines contain a description of $m$ test cases. </p><p>The first line of each test case contains four integers $n, T, a, b$ ($2 \le n \le 2\cdot10^5$, $1 \le T \le 10^9$, $1 \le a &lt; b \le 10^9$)&nbsp;— the number of problems, minutes given for the exam and the time to solve an easy and hard problem, respectively.</p><p>The second line of each test case contains $n$ numbers $0$ or $1$, separated by single space: the $i$-th number means the type of the $i$-th problem. A value of $0$ means that the problem is easy, and a value of $1$ that the problem is hard.</p><p>The third line of each test case contains $n$ integers $t_i$ ($0 \le t_i \le T$), where the $i$-th number means the time at which the $i$-th problem will become mandatory.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>Print the answers to $m$ test cases. For each set, print a single integer&nbsp;— maximal number of points that he can receive, before leaving the exam.</p></div>

## Input

<p>The first line contains the integer $m$ ($1 \le m \le 10^4$)&nbsp;— the number of test cases in the test.</p><p>The next lines contain a description of $m$ test cases. </p><p>The first line of each test case contains four integers $n, T, a, b$ ($2 \le n \le 2\cdot10^5$, $1 \le T \le 10^9$, $1 \le a &lt; b \le 10^9$)&nbsp;— the number of problems, minutes given for the exam and the time to solve an easy and hard problem, respectively.</p><p>The second line of each test case contains $n$ numbers $0$ or $1$, separated by single space: the $i$-th number means the type of the $i$-th problem. A value of $0$ means that the problem is easy, and a value of $1$ that the problem is hard.</p><p>The third line of each test case contains $n$ integers $t_i$ ($0 \le t_i \le T$), where the $i$-th number means the time at which the $i$-th problem will become mandatory.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>Print the answers to $m$ test cases. For each set, print a single integer&nbsp;— maximal number of points that he can receive, before leaving the exam.</p>





```input1
10
3 5 1 3
0 0 1
2 1 4
2 5 2 3
1 0
3 2
1 20 2 4
0
16
6 20 2 5
1 1 0 1 0 0
0 8 2 9 11 6
4 16 3 6
1 0 1 1
8 3 5 6
6 20 3 6
0 1 0 0 1 0
20 11 3 20 16 17
7 17 1 6
1 1 0 1 0 0 0
1 7 0 11 10 15 10
6 17 2 6
0 0 1 0 0 1
7 6 3 7 10 12
5 17 2 5
1 1 1 1 0
17 11 10 6 4
1 1 1 2
0
1
```




```output1
3
2
1
0
1
4
0
1
2
1
```


