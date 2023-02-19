## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Jury initially had a sequence $a$ of length $n$, such that $a_i = i$.</p><p>The jury chose three integers $i$, $j$, $k$, such that $1 \leq i &lt; j &lt; k \leq n$, $j - i &gt; 1$. After that, Jury reversed subsegments $[i, j - 1]$ and $[j, k]$ of the sequence $a$.</p><p>Reversing a subsegment $[l, r]$ of the sequence $a$ means reversing the order of elements $a_l, a_{l+1}, \ldots, a_r$ in the sequence, i.&nbsp;e. $a_l$ is swapped with $a_r$, $a_{l+1}$ is swapped with $a_{r-1}$, etc.</p><p>You are given the number $n$ and you should find $i$, $j$, $k$ after asking some questions.</p><p>In one question you can choose two integers $l$ and $r$ ($1 \leq l \leq r \leq n$) and ask the number of inversions on the subsegment $[l, r]$ of the sequence $a$. You will be given the number of pairs $(i, j)$ such that $l \leq i &lt; j \leq r$, and $a_i &gt; a_j$.</p><p>Find the chosen numbers $i$, $j$, $k$ after at most $40$ questions.</p><p>The numbers $i$, $j$, and $k$ are fixed before the start of your program and do not depend on your queries.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases. Description of the test cases follows.</p><p>The single line of each test case contains a single integer $n$ ($4 \leq n \leq 10^9$). After reading it you should start an interaction process by asking questions for that test case. After giving an answer you should:</p><ul> <li> Terminate your program if that is the last test case. </li><li> Proceed to the next test case otherwise. </li></ul></div><div><h2>Interaction</h2><p>To ask number of inversions on a subsegment $[l, r]$, print "<span class="tex-font-style-tt">? l r</span>", where ($1 \leq l \leq r \leq n$). You can ask at most $40$ questions in each test case. As a result you should read a single integer $x$.</p><ul> <li> If $x = -1$, your program made an invalid question or you exceeded the number of questions for that test case. Your program should terminate immediately (otherwise it can get any verdict instead of "<span class="tex-font-style-tt">Wrong Answer</span>"). </li><li> Otherwise $x$ is equal to the number of inversions on the subsegment $[l, r]$ of the sequence $a$. </li></ul><p>To give the answer, print "<span class="tex-font-style-tt">! i j k</span>", where $i$, $j$, $k$ are the numbers you found. You should continue solving the next test cases or terminate the program after that.</p><p>After printing a question or an answer do not forget to print the end of line and flush the output. Otherwise, you will get an "<span class="tex-font-style-tt">Idleness limit exceeded</span>" verdict. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> See the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To make a hack, use the following format:</p><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases.</p><p>Each of the next $t$ lines contains four integers $n$, $i$, $j$, $k$ ($4 \leq n \leq 10^9$, $1 \leq i &lt; j &lt; k \leq n$, $j - i &gt; 1$).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \leq t \leq 100$) — the number of test cases. Description of the test cases follows.</p><p>The single line of each test case contains a single integer $n$ ($4 \leq n \leq 10^9$). After reading it you should start an interaction process by asking questions for that test case. After giving an answer you should:</p><ul> <li> Terminate your program if that is the last test case. </li><li> Proceed to the next test case otherwise. </li></ul>





```input1
2 
5 

4 

3 

3 

5 

2 

2 

1
```




```output1
? 1 5

? 2 5

? 3 5

! 1 3 5

? 1 5

? 2 5

? 3 5

! 2 4 5
```



## Note

<p>In the first test case, $i = 1$, $j = 3$, $k = 5$, so the sequence $a$ is $[2, 1, 5, 4, 3]$.</p><p>In the second test case, $i = 2$, $j = 4$, $k = 5$, so the sequence $a$ is $[1, 3, 2, 5, 4]$.</p>
