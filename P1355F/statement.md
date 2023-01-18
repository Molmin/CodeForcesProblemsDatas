## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>We have hidden an integer $1 \le X \le 10^{9}$. You <span class="tex-font-style-bf">don't have to</span> guess this number. You have to <span class="tex-font-style-bf">find the number of divisors</span> of this number, and you <span class="tex-font-style-bf">don't even have to find the exact number</span>: your answer will be considered correct if its absolute error is not greater than 7 <span class="tex-font-style-bf">or</span> its relative error is not greater than $0.5$. More formally, let your answer be $ans$ and the number of divisors of $X$ be $d$, then your answer will be considered correct if <span class="tex-font-style-bf">at least one</span> of the two following conditions is true:</p><ul><li> $| ans - d | \le 7$;</li><li> $\frac{1}{2} \le \frac{ans}{d} \le 2$.</li></ul><p>You can make at most $22$ queries. One query consists of one integer $1 \le Q \le 10^{18}$. In response, you will get $gcd(X, Q)$&nbsp;— the greatest common divisor of $X$ and $Q$.</p><p>The number $X$ is fixed before all queries. In other words, <span class="tex-font-style-bf">interactor is not adaptive</span>.</p><p>Let's call the process of guessing the number of divisors of number $X$ a <span class="tex-font-style-it">game</span>. In one test you will have to play $T$ independent games, that is, guess the number of divisors $T$ times for $T$ independent values of $X$.</p></div><div class="input-specification"><p>The first line of input contains one integer $T$ ($1 \le T \le 100$)&nbsp;— the number of games.</p></div><div><h2>Interaction</h2><p>To make a query print a line "<span class="tex-font-style-tt">? Q</span>" ($1 \le Q \le 10^{18}$). After that read one integer $gcd(X, Q)$. You can make no more than $22$ such queries during one game.</p><p>If you are confident that you have figured out the number of divisors of $X$ with enough precision, you can print your answer in "<span class="tex-font-style-tt">! ans</span>" format. $ans$ have to be an integer. If this was the last game, you have to terminate the program, otherwise you have to start the next game immediately. Note that the interactor doesn't print anything in response to you printing answer.</p><p>After printing a query do not forget to output end of line and flush the output. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, use the following format:</p><p>The first line contains one integer $T$ ($1 \le T \le 100$)&nbsp;— the number of games.</p><p>Each of the next $T$ lines contains one integer $X$ ($1 \le X \le 10^{9}$)&nbsp;— the hidden number.</p><p>So the example has the form </p><pre class="verbatim"><br>2<br>998244353<br>4194304<br></pre></div>

## Input

<p>The first line of input contains one integer $T$ ($1 \le T \le 100$)&nbsp;— the number of games.</p>





```input1
2

1

1

1


1024

1048576

4194304
```




```output1
? 982306799268821872

? 230856864650023977

? 134690134760714371

! 5
? 1024

? 1048576

? 1073741824

! 42
```



## Note

<p>Why the limitation for number of queries is 22 exactly? Maybe the problem author is a Taylor Swift fan.</p><p>Let's look at the example.</p><p>In the first game $X = 998\,244\,353$ is hidden. Would be hard to guess this, right? This number is prime, so the number of its divisors is 2. The solution has made several random queries, and all the responses turned out to be 1 (strange things, not even one of three random numbers is divisible by $998\,244\,353$). It's fare to assume that the hidden number doesn't have many divisors, so the solution has answered 5. Why not. This answer will be considered correct since $| 5 - 2 | = 3 \le 7$.</p><p>In the second game $X = 4\,194\,304 = 2^{22}$ is hidden, it has 23 divisors. The solution has made queries $1024 = 2^{10}$, $1\,048\,576 =2^{20}$, $1\,073\,741\,824 = 2^{30}$ and got responses $1024 = 2^{10}$, $1\,048\,576 =2^{20}$, $4\,194\,304 = 2^{22}$, respectively. Then the solution got completely confused and answered the answer to The Ultimate Question of Life, the Universe, and Everything. This answer will be considered correct since $\frac{1}{2} \le \frac{42}{23} \le 2$.</p>
