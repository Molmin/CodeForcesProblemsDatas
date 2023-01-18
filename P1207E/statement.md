## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. Remember to flush your output while communicating with the testing program.</span> You may use <span class="tex-font-style-tt">fflush(stdout)</span> in C++, <span class="tex-font-style-tt">system.out.flush()</span> in Java, <span class="tex-font-style-tt">stdout.flush()</span> in Python or <span class="tex-font-style-tt">flush(output)</span> in Pascal to flush the output. If you use some other programming language, consult its documentation. You may also refer to the guide on interactive problems: <a href="https://codeforces.com/blog/entry/45307">https://codeforces.com/blog/entry/45307</a>.</p><p>The jury picked an integer $x$ not less than $0$ and not greater than $2^{14} - 1$. You have to guess this integer.</p><p>To do so, you may ask no more than $2$ queries. Each query should consist of $100$ integer numbers $a_1$, $a_2$, ..., $a_{100}$ (each integer should be not less than $0$ and not greater than $2^{14} - 1$). In response to your query, the jury will pick one integer $i$ ($1 \le i \le 100$) and tell you the value of $a_i \oplus x$ (the bitwise XOR of $a_i$ and $x$). There is an additional constraint on the queries: all $200$ integers you use in the queries should be distinct.</p><p><span class="tex-font-style-bf">It is guaranteed that the value of $x$ is fixed beforehand in each test, but the choice of $i$ in every query may depend on the integers you send.</span></p></div><div class="output-specification"><p>To give the answer, your program should print one line $!$ $x$ <span class="tex-font-style-it">with a line break in the end</span>. After that, it should flush the output and terminate gracefully.</p></div><div><h2>Interaction</h2><p>Before giving the answer, you may submit no more than $2$ queries. To ask a query, print one line in the following format: $?$ $a_1$ $a_2$ ... $a_{100}$, where every $a_j$ should be an integer from the range $[0, 2^{14} - 1]$. <span class="tex-font-style-it">The line should be ended with a line break character</span>. After submitting a query, flush the output and read the answer to your query — the value of $a_i \oplus x$ for some $i \in [1, 100]$. <span class="tex-font-style-bf">No integer can be used in queries more than once.</span></p><p>If you submit an incorrect query (or ask more than $2$ queries), the answer to it will be one integer $-1$. After receiving such an answer, your program should terminate immediately — otherwise you may receive verdict "Runtime error", "Time limit exceeded" or some other verdict instead of "Wrong answer".</p></div>

## Output

<p>To give the answer, your program should print one line $!$ $x$ <span class="tex-font-style-it">with a line break in the end</span>. After that, it should flush the output and terminate gracefully.</p>





```input1
0
32
```




```output1
? 3 5 6
? 32 24 37
! 5
```



## Note

<p>The example of interaction <span class="tex-font-style-bf">is not correct</span> — you should sumbit <span class="tex-font-style-bf">exactly</span> $100$ integers in each query. Everything else is correct.</p><p><span class="tex-font-style-bf">Hacks are forbidden in this problem</span>.</p>
