## Description

<div><p>Adding two numbers several times is a time-consuming task, so you want to build a robot. The robot should have a string $S = S_1 S_2 \dots S_N$ of $N$ characters on its memory that represents addition instructions. Each character of the string, $S_i$, is either '<span class="tex-font-style-tt">A</span>' or '<span class="tex-font-style-tt">B</span>'.</p><p>You want to be able to give $Q$ commands to the robot, each command is either of the following types: </p><ul> <li> 1 $L$ $R$. The robot should toggle all the characters of $S_i$ where $L \le i \le R$. Toggling a character means changing it to '<span class="tex-font-style-tt">A</span>' if it was previously '<span class="tex-font-style-tt">B</span>', or changing it to '<span class="tex-font-style-tt">B</span>' if it was previously '<span class="tex-font-style-tt">A</span>'. </li><li> 2 $L$ $R$ $A$ $B$. The robot should call $f(L, R, A, B)$ and return two integers as defined in the following pseudocode: <pre class="lstlisting"><code class="prettyprint">    function f(L, R, A, B):<br>      FOR i from L to R<br>        if S[i] = 'A'<br>          A = A + B<br>        else<br>          B = A + B<br>      return (A, B)<br>  </code></pre> </li></ul><p>You want to implement the robot's expected behavior.</p></div><div class="input-specification"><p>Input begins with a line containing two integers: $N$ $Q$ ($1 \le N, Q \le 100\,000$) representing the number of characters in the robot's memory and the number of commands, respectively. The next line contains a string $S$ containing $N$ characters (each either '<span class="tex-font-style-tt">A</span>' or '<span class="tex-font-style-tt">B</span>') representing the initial string in the robot's memory. The next $Q$ lines each contains a command of the following types. </p><ul> <li> 1 $L$ $R$ ($1 \le L \le R \le N$) </li><li> 2 $L$ $R$ $A$ $B$ ($1 \le L \le R \le N$; $0 \le A, B \le 10^9$) </li></ul> There is at least one command of the second type.</div><div class="output-specification"><p>For each command of the second type in the same order as input, output in a line two integers (separated by a single space), the value of $A$ and $B$ returned by $f(L, R, A, B)$, respectively. As this output can be large, you need to modulo the output by $1\,000\,000\,007$.</p></div>

## Input

<p>Input begins with a line containing two integers: $N$ $Q$ ($1 \le N, Q \le 100\,000$) representing the number of characters in the robot's memory and the number of commands, respectively. The next line contains a string $S$ containing $N$ characters (each either '<span class="tex-font-style-tt">A</span>' or '<span class="tex-font-style-tt">B</span>') representing the initial string in the robot's memory. The next $Q$ lines each contains a command of the following types. </p><ul> <li> 1 $L$ $R$ ($1 \le L \le R \le N$) </li><li> 2 $L$ $R$ $A$ $B$ ($1 \le L \le R \le N$; $0 \le A, B \le 10^9$) </li></ul> There is at least one command of the second type.

## Output

<p>For each command of the second type in the same order as input, output in a line two integers (separated by a single space), the value of $A$ and $B$ returned by $f(L, R, A, B)$, respectively. As this output can be large, you need to modulo the output by $1\,000\,000\,007$.</p>





```input1
5 3
ABAAA
2 1 5 1 1
1 3 5
2 2 5 0 1000000000
```




```output1
11 3
0 1000000000
```



## Note

<p><span class="tex-font-style-it">Explanation for the sample input/output #1</span></p><p>For the first command, calling $f(L, R, A, B)$ causes the following: </p><ul> <li> Initially, $A = 1$ and $B = 1$. </li><li> At the end of $i = 1$, $A = 2$ and $B = 1$. </li><li> At the end of $i = 2$, $A = 2$ and $B = 3$. </li><li> At the end of $i = 3$, $A = 5$ and $B = 3$. </li><li> At the end of $i = 4$, $A = 8$ and $B = 3$. </li><li> At the end of $i = 5$, $A = 11$ and $B = 3$. </li></ul> Therefore, $f(L, R, A, B)$ will return $(11, 3)$.<p>For the second command, string $S$ will be updated to "<span class="tex-font-style-tt">ABBBB</span>".</p><p>For the third command, the value of $A$ will always be $0$ and the value of $B$ will always be $1\,000\,000\,000$. Therefore, $f(L, R, A, B)$ will return $(0, 1\,000\,000\,000)$.</p>
