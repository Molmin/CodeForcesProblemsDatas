## Description

<div><p><span class="tex-font-style-it">This is an interactive problem. The only difference between the easy and hard version is the limit on number of questions.</span></p><p>There are $n$ players labelled from $1$ to $n$. <span class="tex-font-style-bf">It is guaranteed that $n$ is a multiple of $3$.</span></p><p>Among them, there are $k$ impostors and $n-k$ crewmates. The number of impostors, $k$, is not given to you. <span class="tex-font-style-bf">It is guaranteed that $\frac{n}{3} &lt; k &lt; \frac{2n}{3}$.</span></p><p>In each question, you can choose three distinct integers $a$, $b$, $c$ ($1 \le a, b, c \le n$) and ask: "Among the players labelled $a$, $b$ and $c$, are there more impostors or more crewmates?" You will be given the integer $0$ if there are more impostors than crewmates, and $1$ otherwise.</p><p>Find the number of impostors $k$ and the indices of players that are impostors after asking at most $2n$ questions.</p><p>The jury is <span class="tex-font-style-bf">adaptive</span>, which means the indices of impostors may not be fixed beforehand and can depend on your questions. It is guaranteed that there is at least one set of impostors which fulfills the constraints and the answers to your questions at any time.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first and only line of each test case contains a single integer $n$ ($6 \le n &lt; 10^4$, $n$ is a multiple of $3$) — the number of players.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^4$.</p></div><div><h2>Interaction</h2><p>For each test case, the interaction starts with reading $n$.</p><p>Then you are allowed to make at most $2n$ questions in the following way:</p><p>"<span class="tex-font-style-tt">? a b c</span>" ($1 \le a, b, c \le n$, $a$, $b$ and $c$ are pairwise distinct).</p><p>After each one, you should read an integer $r$, which is equal to $0$ if there are more impostors than crewmates among players labelled $a$, $b$ and $c$, and equal to $1$ otherwise.</p><p>Answer $-1$ instead of $0$ or $1$ means that you made an invalid query or exceeded the number of queries. Exit immediately after receiving $-1$ and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p><p>When you have found the indices of all impostors, print a single line "<span class="tex-font-style-tt">! </span>" (without quotes), followed by the number of impostors $k$, followed by $k$ integers representing the indices of the impostors. Please note that you must print all this information on the same line. </p><p>After printing the answer, your program must then continue to solve the remaining test cases, or exit if all test cases have been solved.</p><p>After printing the queries and answers do not forget to output end of line and flush the output buffer. Otherwise, you will get the <span class="tex-font-style-tt">Idleness limit exceeded</span> verdict. To do flush use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> Read documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>You cannot make hacks in this problem.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first and only line of each test case contains a single integer $n$ ($6 \le n &lt; 10^4$, $n$ is a multiple of $3$) — the number of players.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^4$.</p>





```input1
2
6

0

1

9

1
```




```output1
? 1 2 3

? 3 4 5

! 3 4 1 2

? 7 1 9

! 4 2 3 6 8
```



## Note

<p>Explanation for example interaction (note that this example only exists to demonstrate the interaction procedure and does not provide any hint for the solution):</p><p>For the first test case:</p><p>Question "<span class="tex-font-style-tt">? 1 2 3</span>" returns $0$, so there are more impostors than crewmates among players $1$, $2$ and $3$.</p><p>Question "<span class="tex-font-style-tt">? 3 4 5</span>" returns $1$, so there are more crewmates than impostors among players $3$, $4$ and $5$.</p><p>Outputting "<span class="tex-font-style-tt">! 3 4 1 2</span>" means that one has found all the impostors, by some miracle. There are $k = 3$ impostors. The players who are impostors are players $4$, $1$ and $2$.</p><p>For the second test case:</p><p>Question "<span class="tex-font-style-tt">? 7 1 9</span>" returns $1$, so there are more crewmates than impostors among players $7$, $1$ and $9$.</p><p>Outputting "<span class="tex-font-style-tt">! 4 2 3 6 8</span>" means that one has found all the impostors, by some miracle. There are $k = 4$ impostors. The players who are impostors are players $2$, $3$, $6$ and $8$.</p>
