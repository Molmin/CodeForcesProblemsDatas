## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>There was a tournament consisting of $2^n$ contestants. The $1$-st contestant competed with the $2$-nd, the $3$-rd competed with the $4$-th, and so on. After that, the winner of the first match competed with the winner of second match, etc. The tournament ended when there was only one contestant left, who was declared the winner of the tournament. Such a tournament scheme is known as the single-elimination tournament.</p><p>You don't know the results, but you want to find the winner of the tournament. In one query, you select two integers $a$ and $b$, which are the indices of two contestants. The jury will return $1$ if $a$ won more matches than $b$, $2$ if $b$ won more matches than $a$, or $0$ if their number of wins was equal.</p><p>Find the winner in no more than $\left \lceil \frac{1}{3} \cdot 2^{n + 1} \right \rceil$ queries. Here $\lceil x \rceil$ denotes the value of $x$ rounded up to the nearest integer.</p><p>Note that the tournament is long over, meaning that the results are fixed and do not depend on your queries.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 2^{14}$) — the number of test cases.</p><p>The only line of input contains a single integer $n$ ($1 \leq n \leq 17$).</p><p>It is guaranteed that the sum of $2^n$ over all test cases does not exceed $2^{17}$.</p></div><div><h2>Interaction</h2><p>The interaction for each test case begins by reading the integer $n$.</p><p>To make a query, output "<span class="tex-font-style-tt">? a b</span>" ($1 \leq a, b \leq 2^n$) without quotes. Afterwards, you should read one single integer — the answer for your query. You can make at most $\left \lceil \frac{1}{3} \cdot 2^{n + 1} \right \rceil$ such queries in each test case.</p><p>If you receive the integer $-1$ instead of an answer or a valid value of $n$, it means your program has made an invalid query, has exceed the limit of queries, or has given incorrect answer on the previous test case. Your program must terminate immediately to receive a <span class="tex-font-style-tt">Wrong Answer</span> verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>When you are ready to give the final answer, output "<span class="tex-font-style-tt">! x</span>" ($1 \leq x \leq 2^n$) without quotes — the winner of the tournament. Giving this answer does not count towards the limit of queries. After solving a test case, your program should move to the next one immediately. After solving all test cases, your program should be terminated immediately.</p><p>After printing a query or the answer do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush(</span>) in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, use the following format.</p><p>The first line contains an integer $t$ ($1 \leq t \leq 2^{14}$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 17$).</p><p>The second line of each test case contains $2^n$ numbers on a line — the number of wins of each participant. There should be a sequence of matches that is consistent with the number of wins.</p><p>The sum of $2^n$ should not exceed $2^{17}$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 2^{14}$) — the number of test cases.</p><p>The only line of input contains a single integer $n$ ($1 \leq n \leq 17$).</p><p>It is guaranteed that the sum of $2^n$ over all test cases does not exceed $2^{17}$.</p>





```input1
1
3

2

0

2
```




```output1
? 1 4

? 1 6

? 5 7

! 7
```



## Note

<p>The tournament in the first test case is shown below. The number of wins is $[1,0,0,2,0,1,3,0]$.</p><center> <img class="tex-graphics" src="file://1OF9fJ8N.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">In this example, the winner is the $7$-th contestant.</span> </center>
