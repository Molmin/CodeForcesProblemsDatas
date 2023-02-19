## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>There is a positive integer $1 \le x \le 10^9$ that you have to guess.</p><p>In one query you can choose two positive integers $a \neq b$. As an answer to this query you will get $\gcd(x + a, x + b)$, where $\gcd(n, m)$ is the <a href="https://en.wikipedia.org/wiki/Greatest common divisor">greatest common divisor</a> of the numbers $n$ and $m$.</p><p>To guess one hidden number $x$ you are allowed to make no more than $30$ queries.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \le t \le 1000$) denoting the number of test cases.</p><p>The integer $x$ that you have to guess satisfies the constraints: ($1 \le x \le 10^9$).</p></div><div><h2>Interaction</h2><p>The hidden number $x$ is fixed before the start of the interaction and does not depend on your queries.</p><p>To guess each $x$ you can make no more than $30$ queries in the following way:</p><ul> <li> "<span class="tex-font-style-tt">? a b</span>" ($1 \le a, b \le 2 \cdot 10^9$, $a \neq b$). </li></ul><p>For this query you will get $\gcd(x + a, x + b)$.</p><p>When you know $x$, print a single line in the following format.</p><ul> <li> "<span class="tex-font-style-tt">! x</span>" ($1 \le x \le 10^9$). </li></ul><p>After that continue to solve the next test case.</p><p>If you ask more than $30$ queries for one $x$ or make an invalid query, the interactor will terminate immediately and your program will receive verdict <span class="tex-font-style-tt">Wrong Answer</span>.</p><p>After printing each query do not forget to output end of line and flush the output buffer. Otherwise, you will get the <span class="tex-font-style-tt">Idleness limit exceeded</span> verdict. To do flush use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> Read documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To use hacks, use the following format of tests:</p><p>The first line should contain a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case should contain a single integer $x$ ($1 \le x \le 10^9$) denoting the integer $x$ that should be guessed.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \le t \le 1000$) denoting the number of test cases.</p><p>The integer $x$ that you have to guess satisfies the constraints: ($1 \le x \le 10^9$).</p>





```input1
2

1

8


1
```




```output1
? 1 2

? 12 4

! 4
? 2000000000 1999999999

! 1000000000
```



## Note

<p>The first hidden number is $4$, that's why the answers for the queries are:</p><p>"<span class="tex-font-style-tt">? 1 2</span>"&nbsp;— $\gcd(4 + 1, 4 + 2) = \gcd(5, 6) = 1$.</p><p>"<span class="tex-font-style-tt">? 12 4</span>"&nbsp;— $\gcd(4 + 12, 4 + 4) = \gcd(16, 8) = 8$.</p><p>The second hidden number is $10^9$, that's why the answer for the query is:</p><p>"<span class="tex-font-style-tt">? 2000000000 1999999999</span>"&nbsp;— $\gcd(3 \cdot 10^9, 3 \cdot 10^9 - 1) = 1$.</p><p><span class="tex-font-style-it">These queries are made only for understanding the interaction and are not enough for finding the true $x$.</span></p>
