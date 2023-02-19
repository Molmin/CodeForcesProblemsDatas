## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The only difference is that here $2\leq k\leq 100$. You can make hacks only if both the versions of the problem are solved.</span></p><p><span class="tex-font-style-bf">This is an interactive problem!</span></p><p>Every decimal number has a base $k$ equivalent. The individual digits of a base $k$ number are called $k$-its. Let's define the $k$-itwise XOR of two $k$-its $a$ and $b$ as $(a + b)\bmod k$.</p><p>The $k$-itwise XOR of two base $k$ numbers is equal to the new number formed by taking the $k$-itwise XOR of their corresponding $k$-its. The $k$-itwise XOR of two decimal numbers $a$ and $b$ is denoted by $a\oplus_{k} b$ and is equal to the decimal representation of the $k$-itwise XOR of the base $k$ representations of $a$ and $b$. All further numbers used in the statement below are in decimal unless specified.</p><p>You have hacked the criminal database of Rockport Police Department (RPD), also known as the Rap Sheet. But in order to access it, you require a password. You don't know it, but you are quite sure that it lies between $0$ and $n-1$ inclusive. So, you have decided to guess it. Luckily, you can try at most $n$ times without being blocked by the system. But the system is adaptive. Each time you make an incorrect guess, it changes the password. Specifically, if the password before the guess was $x$, and you guess a different number $y$, then the system changes the password to a number $z$ such that $x\oplus_{k} z=y$. Guess the password and break into the system.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1\leq t\leq 10\,000$) denoting the number of test cases. $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ ($1\leq n\leq 2\cdot 10^5$) and $k$ $(2\leq k\leq 100)$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div><h2>Interaction</h2><p>For each test case, first read two integers $n$ and $k$. Then you may ask up to $n$ queries.</p><p>For each query, print a single integer $y$ ($0\leq y\leq 2\cdot 10^7$). Let the current password be $x$. After that, read an integer $r$.</p><p>If $x=y$, you will read $r=1$ and the test case is solved. You must then continue solving the remaining test cases.</p><p>Else, you will read $r=0$. At this moment the password is changed to a number $z$ such that $x\oplus_{k} z=y$.</p><p>After printing a query, do not forget to output the end of line and flush the output. Otherwise, you will get the <span class="tex-font-style-tt">Idleness limit exceeded</span> verdict.</p><p>To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p>If you ask an invalid query or exceed $n$ queries, you will read $r=-1$ and you will receive the <span class="tex-font-style-tt">Wrong Answer</span> verdict. Make sure to exit immediately to avoid unexpected verdicts.</p><p>Note that the interactor is <span class="tex-font-style-bf">adaptive</span>. That is, the original password is not fixed in the beginning and may depend on your queries. But it is guaranteed that at any moment there is at least one initial password such that all the answers to the queries are consistent.</p><p><span class="tex-font-style-bf">Hacks:</span></p><p>To use hacks, use the following format of tests:</p><p>The first line should contain a single integer $t$ ($1\leq t\leq 10\,000$) — the number of test cases.</p><p>The first and only line of each test case should contain two integers $n$ ($1\leq n\leq 2\cdot 10^5$) and $k$ ($2\leq k\leq 100$) denoting the number of queries and the base respectively. The optimal original password is automatically decided by the adaptive interactor.</p><p>You must ensure that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1\leq t\leq 10\,000$) denoting the number of test cases. $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ ($1\leq n\leq 2\cdot 10^5$) and $k$ $(2\leq k\leq 100)$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>





```input1
2
5 2

0

0

1
5 3

0

0

1
```




```output1
3

4

5


1

4

6
```



## Note

<p><span class="tex-font-style-bf">Test Case 1:</span></p><p>In this case, the hidden password is $2$.</p><p>The first query is $3$. It is not equal to the current password. So, $0$ is returned, and the password is changed to $1$ since $2\oplus_2 1=3$.</p><p>The second query is $4$. It is not equal to the current password. So, $0$ is returned, and the password is changed to $5$ since $1\oplus_2 5=4$.</p><p>The third query is $5$. It is equal to the current password. So, $1$ is returned, and the job is done.</p><p><span class="tex-font-style-bf">Test Case 2:</span></p><p>In this case, the hidden password is $3$.</p><p>The first query is $1$. It is not equal to the current password. So, $0$ is returned, and the password is changed to $7$ since $3\oplus_3 7=1$. $[3=(10)_3$, $7=(21)_3$, $1=(01)_3$ and $(10)_3\oplus_3 (21)_3 = (01)_3]$.</p><p>The second query is $4$. It is not equal to the current password. So, $0$ is returned, and the password is changed to $6$ since $7\oplus_3 6=4$. $[7=(21)_3$, $6=(20)_3$, $4=(11)_3$ and $(21)_3\oplus_3 (20)_3 = (11)_3]$.</p><p>The third query is $6$. It is equal to the current password. So, $1$ is returned, and the job is done.</p><p>Note that these initial passwords are taken just for the sake of explanation. In reality, the grader might behave differently because it is adaptive.</p>
