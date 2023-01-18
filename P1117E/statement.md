## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. Remember to flush your output while communicating with the testing program.</span> You may use <span class="tex-font-style-tt">fflush(stdout)</span> in C++, <span class="tex-font-style-tt">system.out.flush()</span> in Java, <span class="tex-font-style-tt">stdout.flush()</span> in Python or <span class="tex-font-style-tt">flush(output)</span> in Pascal to flush the output. If you use some other programming language, consult its documentation. You may also refer to the guide on interactive problems: <a href="https://codeforces.com/blog/entry/45307">https://codeforces.com/blog/entry/45307</a>.</p><p>You are given a string $t$ consisting of $n$ lowercase Latin letters. This string was cyphered as follows: initially, the jury had a string $s$ consisting of $n$ lowercase Latin letters. Then they applied a sequence of no more than $n$ (possibly zero) operations. $i$-th operation is denoted by two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$), and means swapping two elements of the string with indices $a_i$ and $b_i$. All operations were done in the order they were placed in the sequence. For example, if $s$ is <span class="tex-font-style-tt">xyz</span> and $2$ following operations are performed: $a_1 = 1, b_1 = 2$; $a_2 = 2, b_2 = 3$, then after the first operation the current string is <span class="tex-font-style-tt">yxz</span>, and after the second operation the current string is <span class="tex-font-style-tt">yzx</span>, so $t$ is <span class="tex-font-style-tt">yzx</span>.</p><p>You are asked to restore the original string $s$. Unfortunately, you have no information about the operations used in the algorithm (you don't even know if there were any operations in the sequence). But you may run the same sequence of operations on any string you want, provided that it contains only lowercase Latin letters and its length is $n$, and get the resulting string after those operations.</p><p>Can you guess the original string $s$ asking the testing system to run the sequence of swaps no more than $3$ times?</p><p><span class="tex-font-style-bf">The string $s$ and the sequence of swaps are fixed in each test; the interactor doesn't try to adapt the test to your solution</span>.</p></div><div class="input-specification"><p>Initially the testing system sends one string $t$, consisting of lowercase Latin letters ($1 \le |t| = n \le 10^4$).</p></div><div class="output-specification"><p>To give the answer, your program should print one line $!$ $s$ <span class="tex-font-style-it">with a line break in the end</span>. After that, it should flush the output and terminate gracefully.</p></div><div><h2>Interaction</h2><p>Before giving the answer, you may submit no more than $3$ queries. To ask a query, print one line in the following format: $?$ $s'$, where $s'$ should be a string consisting of exaclty $n$ lowercase Latin letters. <span class="tex-font-style-it">The line should be ended with a line break character</span>. After submitting a query, flush the output and read the answer to your query — a string $t'$ consisting of $n$ lowercase Latin letters, which is the result of applying the sequence of swaps to string $s'$. This string will be given on a separate line ended by a line break character.</p><p>If you submit an incorrect query (or ask more than $3$ queries), the answer to it will be one string <span class="tex-font-style-tt">0</span>. After receiving such an answer, your program should terminate immediately — otherwise you may receive verdict "Runtime error", "Time limit exceeded" or some other verdict instead of "Wrong answer".</p></div>

## Input

<p>Initially the testing system sends one string $t$, consisting of lowercase Latin letters ($1 \le |t| = n \le 10^4$).</p>

## Output

<p>To give the answer, your program should print one line $!$ $s$ <span class="tex-font-style-it">with a line break in the end</span>. After that, it should flush the output and terminate gracefully.</p>





```input1
yzx
aab
baa
aba
```




```output1
? baa
? aba
? aab
! xyz
```



## Note

<p>In the sample, the testcase described in the statement is used. The participant asks the first query with string <span class="tex-font-style-tt">baa</span>, which is transformed to <span class="tex-font-style-tt">aab</span>. The second query contains string <span class="tex-font-style-tt">aba</span>, which is transformed to <span class="tex-font-style-tt">baa</span>. The third query contains string <span class="tex-font-style-tt">aab</span>, which is transformed to <span class="tex-font-style-tt">aba</span>. The participant can deduce that the initial string $s$ was <span class="tex-font-style-tt">xyz</span>.</p><p><span class="tex-font-style-bf">Note for hacking phase:</span></p><p>To submit a test in hacking phase, you should provide it in the following format:</p><p>The first line should contain the string $s$ you guess, consisting of $n \in [1, 10000]$ lowercase Latin letters.</p><p>The second line should contain $k$ ($0 \le k \le n$) — the number of swap operations in the sequence.</p><p>Then $k$ lines should follow, $i$-th of them should denote $i$-th operation with two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$).</p><p>For example, the sample test would look like that:</p><p><span class="tex-font-style-tt">xyz</span></p><p><span class="tex-font-style-tt">2</span></p><p><span class="tex-font-style-tt">1 2</span></p><p><span class="tex-font-style-tt">2 3</span></p>
