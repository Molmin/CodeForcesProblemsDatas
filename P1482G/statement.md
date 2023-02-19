## Description

<div><p>Gustaw is the chief bank manager in a huge bank. He has unlimited access to the database system of the bank, in a few clicks he can move any amount of money from the bank's reserves to his own private account. However, the bank uses some fancy AI fraud detection system that makes stealing more difficult.</p><p>Gustaw knows that the anti-fraud system just detects any operation that exceeds some fixed limit $M$ euros and these operations are checked manually by a number of clerks. Thus, any fraud operation exceeding this limit is detected, while any smaller operation gets unnoticed.</p><p>Gustaw doesn't know the limit $M$ and wants to find it out. In one operation, he can choose some integer $X$ and try to move $X$ euros from the bank's reserves to his own account. Then, the following happens. </p><ul> <li> If $X \le M$, the operation is unnoticed and Gustaw's account balance raises by $X$ euros. </li><li> Otherwise, if $X &gt; M$, the fraud is detected and cancelled. Moreover, Gustaw has to pay $X$ euros from his own account as a fine. If he has less than $X$ euros on the account, he is fired and taken to the police. </li></ul><p>Initially Gustaw has $1$ euro on his account. Help him find the exact value of $M$ in no more than $105$ operations without getting him fired.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$).</p><p>For each test case, there is no input prior to your first query, but you can be sure that $M$ is integer, and $0 \le M \le 10^{14}$.</p></div><div class="output-specification"><p>For each test case, when you know the exact value of $M$, print a single line with format "<span class="tex-font-style-tt">!</span> $M$". After that your program should proceed to the next test case or terminate, if it is the last one.</p></div><div><h2>Interaction</h2><p>When you want to make an operation, print a single line with format "<span class="tex-font-style-tt">?</span> $X$", denoting that you try to move $X$ euros ($1 \le X \le 10^{14}$). As a response, read a single line that can take the following values: </p><ul> <li> "<span class="tex-font-style-tt">Lucky!</span>", if $X \le M$. Your balance raises by $X$. </li><li> "<span class="tex-font-style-tt">Fraudster!</span>", if $X &gt; M$. Your balance decreases by $X$. </li><li> "<span class="tex-font-style-tt">Fired!</span>", if $X &gt; M$, but you can't pay $X$ euros of fine. In this case your program must terminate immediately. You also get this response if you exceed the number of queries. </li></ul><p>You can make at most $105$ such queries in each test case.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To make a hack, prepare an input in the following format.</p><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case is described with a line containing a single integer $M$ ($0 \le M \le 10^{14}$).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$).</p><p>For each test case, there is no input prior to your first query, but you can be sure that $M$ is integer, and $0 \le M \le 10^{14}$.</p>

## Output

<p>For each test case, when you know the exact value of $M$, print a single line with format "<span class="tex-font-style-tt">!</span> $M$". After that your program should proceed to the next test case or terminate, if it is the last one.</p>





```input1
1

Lucky!

Lucky!

Lucky!

Lucky!

Lucky!

Fraudster!
```




```output1
? 1

? 2

? 3

? 4

? 5

? 6

! 5
```



## Note

<p>In the example $M = 5$, so the operation with $X = 6$ is detected. At this moment, Gustaw's balance is $16$ euros, so he just pays fine.</p>
