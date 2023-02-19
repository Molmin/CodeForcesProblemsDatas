## Description

<div><p>Alperen is standing at the point $(0,0)$. He is given a string $s$ of length $n$ and performs $n$ moves. The $i$-th move is as follows: </p><ul> <li> if $s_i = \texttt{L}$, then move one unit left; </li><li> if $s_i = \texttt{R}$, then move one unit right; </li><li> if $s_i = \texttt{U}$, then move one unit up; </li><li> if $s_i = \texttt{D}$, then move one unit down. </li></ul> <center> <img class="tex-graphics" src="file://Ru6Cjlyb.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">If Alperen starts at the center point, he can make the four moves shown.</span> </center> There is a candy at $(1,1)$ (that is, one unit above and one unit to the right of Alperen's starting point). You need to determine if Alperen ever passes the candy. <center> <img class="tex-graphics" src="file://PL3W5KI8.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Alperen's path in the first test case.</span> </center></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of characters $\texttt{L}$, $\texttt{R}$, $\texttt{D}$, and $\texttt{U}$, denoting the moves Alperen makes.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alperen passes the candy, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 50$)&nbsp;— the length of the string.</p><p>The second line of each test case contains a string $s$ of length $n$ consisting of characters $\texttt{L}$, $\texttt{R}$, $\texttt{D}$, and $\texttt{U}$, denoting the moves Alperen makes.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if Alperen passes the candy, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11,14,15
7
7
UUURDDL
2
UR
8
RRRUUDDD
3
LLL
4
DUUR
5
RUDLL
11
LLLLDDRUDRD
```




```output1
YES
YES
NO
NO
YES
YES
NO
```



## Note

<p>In the first test case, Alperen follows the path $$(0,0) \overset{\texttt{U}}{\to} (0,1) \overset{\texttt{U}}{\to} (0,2) \overset{\texttt{U}}{\to} (0,3) \overset{\texttt{R}}{\to} (1,3) \overset{\texttt{D}}{\to} (1,2) \overset{\texttt{D}}{\to} \color{green}{\mathbf{(1,1)}} \overset{\texttt{L}}{\to} (0,1).$$ Note that Alperen doesn't need to end at the candy's location of $(1,1)$, he just needs to pass it at some point.</p><p>In the second test case, Alperen follows the path $$(0,0) \overset{\texttt{U}}{\to} (0,1) \overset{\texttt{R}}{\to} \color{green}{\mathbf{(1,1)}}.$$</p><p>In the third test case, Alperen follows the path $$(0,0) \overset{\texttt{R}}{\to} (1,0) \overset{\texttt{R}}{\to} (2,0) \overset{\texttt{R}}{\to} (3,0) \overset{\texttt{U}}{\to} (3,1) \overset{\texttt{U}}{\to} (3,2) \overset{\texttt{D}}{\to} (3,1) \overset{\texttt{D}}{\to} (3,0) \overset{\texttt{D}}{\to} (3,-1).$$</p><p>In the fourth test case, Alperen follows the path $$(0,0) \overset{\texttt{L}}{\to} (-1,0) \overset{\texttt{L}}{\to} (-2,0) \overset{\texttt{L}}{\to} (-3,0).$$</p>
