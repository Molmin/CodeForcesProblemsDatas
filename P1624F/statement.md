## Description

<div><p><span class="tex-font-style-bf">This problem is interactive.</span></p><p>We decided to play a game with you and guess the number $x$ ($1 \le x &lt; n$), where you know the number $n$.</p><p>You can make queries like this:</p><ul><li> <span class="tex-font-style-tt">+ c</span>: this command assigns $x = x + c$ ($1 \le c &lt; n$) and then returns you the value $\lfloor\frac{x}{n}\rfloor$ ($x$ divide by $n$ and round down).</li></ul><p>You win if you guess the current number with no more than $10$ queries.</p></div><div><h2>Interaction</h2><p>The interaction begins by reading an integer $n$ ($2 &lt; n \le 1000$), which is written in the input data on its own line.</p><p>Then you can make no more than $10$ queries. To make a query, print on a separate line:</p><ul> <li> <span class="tex-font-style-tt">+ c</span>: this command will assign $x = x + c$ ($1 \le c &lt; n$) and then print $\lfloor\frac{x}{n}\rfloor$ (divide $x$ by $n$ and round down) on a separate line. </li></ul> <p>Print the answer, like the queries, on a separate line. The answer doesn't count in number of queries. To output it, use the following format:</p><ul> <li> <span class="tex-font-style-tt">! x</span>: the current value of $x$. </li></ul><p>After that, your program should exit.</p><p>You have to use a <span class="tex-font-style-tt">flush</span> operation right after printing each line. For example, in C++ you should use the function <span class="tex-font-style-tt">fflush(stdout)</span>, in Java — <span class="tex-font-style-tt">System.out.flush()</span>, in Pascal — <span class="tex-font-style-tt">flush(output)</span> and in Python — <span class="tex-font-style-tt">sys.stdout.flush()</span>.</p><p>Note that the interactor is not responsive.</p><p>To make a hack, use the following format: a single line must contain two numbers $x$ and $n$, separated by a space.</p></div>





```input1
3

1
```




```input2
5

0

0

1
```




```input3
10

0

0

1

2
```




```output1
+ 1

! 3
```




```output2
+ 1

+ 1

+ 1

! 5
```




```output3
+ 2

+ 2

+ 3

+ 8

! 20
```



## Note

<p>In the first sample initially $x = 2$. After the first query $x = 3$, $\lfloor\frac{x}{n}\rfloor = 1$.</p><p>In the second sample also initially $x = 2$. After the first query $x = 3$, $\lfloor\frac{x}{n}\rfloor = 0$. After the second query $x = 4$, $\lfloor\frac{x}{n}\rfloor = 0$. After the third query $x=5$, $\lfloor\frac{x}{n}\rfloor = 1$.</p>
