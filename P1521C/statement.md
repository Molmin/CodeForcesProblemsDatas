## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem!</span></p><p>Nastia has a hidden permutation $p$ of length $n$ consisting of integers from $1$ to $n$. You, for some reason, want to figure out the permutation. To do that, you can give her an integer $t$ ($1 \le t \le 2$), two <span class="tex-font-style-bf">different</span> indices $i$ and $j$ ($1 \le i, j \le n$, $i \neq j$), and an integer $x$ ($1 \le x \le n - 1$). </p><p>Depending on $t$, she will answer: </p><ul> <li> $t = 1$: $\max{(\min{(x, p_i)}, \min{(x + 1, p_j)})}$; </li><li> $t = 2$: $\min{(\max{(x, p_i)}, \max{(x + 1, p_j)})}$. </li></ul><p>You can ask Nastia <span class="tex-font-style-bf">at most</span> $\lfloor \frac {3 \cdot n} { 2} \rfloor + 30$ times. It is guaranteed that she will <span class="tex-font-style-bf">not</span> change her permutation depending on your queries. Can you guess the permutation?</p></div><div class="input-specification"><p>The input consists of several test cases. In the beginning, you receive the integer $T$ ($1 \le T \le 10\,000$)&nbsp;— the number of test cases.</p><p>At the beginning of each test case, you receive an integer $n$ ($3 \le n \le 10^4$)&nbsp;— the length of the permutation $p$.</p><p>It's guaranteed that the permutation is fixed beforehand and that the sum of $n$ in one test doesn't exceed $2 \cdot 10^4$.</p></div><div><h2>Interaction</h2><p>To ask a question, print "<span class="tex-font-style-tt">?</span> $t$ $i$ $j$ $x$" ($t = 1$ or $t = 2$, $1 \le i, j \le n$, $i \neq j$, $1 \le x \le n - 1$) Then, you should read the answer.</p><p>If we answer with $−1$ instead of a valid answer, that means you exceeded the number of queries or made an invalid query. Exit immediately after receiving $−1$ and you will see the Wrong Answer verdict. Otherwise, you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>To print the answer, print "<span class="tex-font-style-tt">!</span> $p_1$ $p_2$ $\ldots$ $p_{n}$ (without quotes). <span class="tex-font-style-bf">Note that answering doesn't count as one of the $\lfloor \frac {3 \cdot n} {2} \rfloor + 30$ queries</span>.</p><p>After printing a query or printing the answer, do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> See the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack the solution, use the following test format.</p><p>The first line should contain a single integer $T$ ($1 \le T \le 10\,000$)&nbsp;— the number of test cases.</p><p>For each test case in the first line print a single integer $n$ ($3 \le n \le 10^4$)&nbsp;— the length of the hidden permutation $p$.</p><p>In the second line print $n$ space-separated integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$), where $p$ is permutation.</p><p>Note that the sum of $n$ over all test cases should not exceed $2 \cdot 10^4$.</p></div>

## Input

<p>The input consists of several test cases. In the beginning, you receive the integer $T$ ($1 \le T \le 10\,000$)&nbsp;— the number of test cases.</p><p>At the beginning of each test case, you receive an integer $n$ ($3 \le n \le 10^4$)&nbsp;— the length of the permutation $p$.</p><p>It's guaranteed that the permutation is fixed beforehand and that the sum of $n$ in one test doesn't exceed $2 \cdot 10^4$.</p>





```input1
2
4

3

2

5

3
```




```output1
? 2 4 1 3

? 1 2 4 2

! 3 1 4 2

? 2 3 4 2

! 2 5 3 4 1
```



## Note

<p>Consider the first test case.</p><p>The hidden permutation is $[3, 1, 4, 2]$.</p><p>We print: "<span class="tex-font-style-tt">?</span> $2$ $4$ $1$ $3$" and get back $\min{(\max{(3, p_4}), \max{(4, p_1)})} = 3$.</p><p>We print: "<span class="tex-font-style-tt">?</span> $1$ $2$ $4$ $2$" and get back $\max{(\min{(2, p_2)}, \min{(3, p_4)})} = 2$.</p><p>Consider the second test case.</p><p>The hidden permutation is $[2, 5, 3, 4, 1]$.</p><p>We print: "<span class="tex-font-style-tt">?</span> $2$ $3$ $4$ $2$" and get back $\min{(\max{(2, p_3}), \max{(3, p_4)})} = 3$.</p>
