## Description

<div><p><span class="tex-font-style-bf">The only difference between this problem and the other two versions is the maximum number of queries. In this version, you are allowed to ask at most $\mathbf{20}$ queries. You can make hacks only if all versions of the problem are solved.</span></p><p><span class="tex-font-style-it">This is an interactive problem</span>.</p><p><span class="tex-font-style-it">"Everybody! Doremy's Perfect Data Structure Class is about to start! Come and do your best if you want to have as much IQ as me!" In today's Data Structure class, Doremy is teaching everyone a powerful data structure&nbsp;— Doremy tree! Now she gives you a quiz to prove that you are paying attention in class.</span></p><p>Given an array $a$ of length $m$, Doremy tree supports the query $Q(l,r,k)$, where $1 \leq l \leq r \leq m$ and $1 \leq k \leq m$, which returns the number of distinct integers in the array $\left[\lfloor\frac{a_l}{k} \rfloor, \lfloor\frac{a_{l+1}}{k} \rfloor, \ldots, \lfloor\frac{a_r}{k} \rfloor\right]$.</p><p>Doremy has a secret permutation $p$ of integers from $1$ to $n$. You can make queries, in one query, you give $3$ integers $l,r,k$ ($1 \leq l \leq r \leq n$, $1 \leq k \leq n$) and receive the value of $Q(l,r,k)$ for the array $p$. Can you find the index $y$ ($1 \leq y \leq n$) such that $p_y=1$ in <span class="tex-font-style-bf">at most</span> $\mathbf{20}$ queries?</p><p>Note that the permutation $p$ is fixed before any queries are made.</p></div><div><h2>Interaction</h2><p>You begin the interaction by reading an integer $n$ ($3 \le n \le 1024$) in the first line&nbsp;— the length of the permutation.</p><p>To make a query, you should output </p><ul> <li> "? $l\ r\ k$" ($1 \leq l \leq r \leq n$, $1 \leq k \leq n$) </li></ul> in a separate line. After each query, you should read an integer $x$&nbsp;— the value of $Q(l,r,k)$ for $p$. In this version of the problem, you can make at most $20$ such queries.<p>To give the answer, you should output </p><ul> <li> "! $y$" ($1 \leq y \leq n$) </li></ul> in a separate line, where $p_y=1$.<p>After printing a query or the answer, do not forget to output the end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush(</span>) in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf"><span class="tex-font-style-section">Hacks Format</span></span></p><p>The first line of the hack contains an integer $n$ ($3 \le n \le 1024$)&nbsp;— the length of the permutation.</p><p>The second line of the hack contains $n$ distinct integers $p_1,p_2,\ldots,p_n$ ($1 \le p_i\le n$)&nbsp;— the permutation.</p></div>





```input1
5

2

2

1

3
```




```output1
? 1 3 4

? 3 5 3

? 3 4 5

? 3 5 2

! 4
```



## Note

<p>The permutation in the example is $[3,5,2,1,4]$.</p><p>The input and output for example illustrate possible interaction on that test (empty lines are inserted only for clarity).</p><p>In this interaction process:</p><ul> <li> For the first query, $\lfloor\frac{3}{4}\rfloor=0,\lfloor\frac{5}{4}\rfloor=1,\lfloor\frac{2}{4}\rfloor=0$, so the answer is $2$.</li><li> For the second query, $\lfloor\frac{2}{3}\rfloor=0,\lfloor\frac{1}{3}\rfloor=0,\lfloor\frac{4}{3}\rfloor=1$, so the answer is still $2$.</li><li> For the third query, $\lfloor\frac{2}{5}\rfloor=0,\lfloor\frac{1}{5}\rfloor=0$, so the answer is $1$.</li><li> For the fourth query, $\lfloor\frac{2}{2}\rfloor=1,\lfloor\frac{1}{2}\rfloor=0,\lfloor\frac{4}{2}\rfloor=2$, so the answer is $3$. </li></ul><p>The correct answer is got after $4$ queries, so this process will be judged correct.</p>
