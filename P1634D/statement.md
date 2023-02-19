## Description

<div><center> <img class="tex-graphics" src="file://RmnsI4jn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>We picked an array of whole numbers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$) and concealed <span class="tex-font-style-bf">exactly one</span> zero in it! Your goal is to find the location of this zero, that is, to find $i$ such that $a_i = 0$.</p><p>You are allowed to make several queries to guess the answer. For each query, you can think up three distinct indices $i, j, k$, and we will tell you the value of $\max(a_i, a_j, a_k) - \min(a_i, a_j, a_k)$. In other words, we will tell you the difference between the maximum and the minimum number among $a_i$, $a_j$ and $a_k$.</p><p>You are allowed to make no more than $2 \cdot n - 2$ queries, and after that you have two tries to guess where the zero is. That is, you have to tell us two numbers $i$ and $j$ and you win if $a_i = 0$ or $a_j = 0$.</p><p>Can you guess where we hid the zero?</p><p>Note that the array in each test case is fixed beforehand and will not change during the game. In other words, the interactor is not adaptive.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). Description of the test cases follows.</p><p>The first and only line of each test case contains an integer $n$ ($4 \le n \le 1000$)&nbsp;— the length of the array that we picked.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3000$.</p></div><div><h2>Interaction</h2><p>For each test case, the interaction starts with reading $n$.</p><p>To make a query, print "<span class="tex-font-style-tt">? $i$ $j$ $k$</span>" (without quotes, $1 \le i, j, k \le n$, indices must be distinct). Then you should read our response from standard input, that is, $\max(a_i, a_j, a_k) - \min(a_i, a_j, a_k)$.</p><p>If the response is $-1$, it means your program has made an invalid query or has run out of tries. Your program must terminate immediately after reading $-1$, and you will get a verdict <span class="tex-font-style-tt">Wrong answer</span>. Otherwise you may get any verdict, because the program will continue reading from the closed stream. Note that if the query is correct, the answer will never be $-1$ because $\max(a_i, a_j, a_k) - \min(a_i, a_j, a_k) \geq 0$.</p><p>To give the final answer, print "<span class="tex-font-style-tt">! $i$ $j$</span>" (without the quotes). Printing the same number twice (that is, $i = j$) is allowed. Note that giving this answer is not counted towards the limit of $2 \cdot n - 2$ queries. After that, your program must continue to solve the remaining test cases, or exit if all test cases have been solved.</p><p>After printing a query, don't forget to output line feed and flush the output buffer. Otherwise you will get the verdict <span class="tex-font-style-tt">Idleness limit exceeded</span>. To flush the buffer, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> Read documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>The first line must contain an integer $t$ ($1 \le t \le 500$)&nbsp;— the count of test cases.</p><p>The first line of each test case must contain an integer $n$ ($4 \le n \le 1000$)&nbsp;— the length of the hidden array.</p><p>The second line of each test case must contain $n$ integers separated by spaces&nbsp;— $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$). There must also be <span class="tex-font-style-bf">exactly one</span> zero in this array.</p><p>The sum of $n$ over all test cases must not exceed $3000$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 500$). Description of the test cases follows.</p><p>The first and only line of each test case contains an integer $n$ ($4 \le n \le 1000$)&nbsp;— the length of the array that we picked.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3000$.</p>





```input1
1

4

2

3

3

2
```




```output1
? 1 2 3

? 2 3 4

? 3 4 1

? 4 1 2

! 2 3
```



## Note

<p>Array from sample: $[1, 2, 0, 3]$.</p>
