## Description

<div><p>A number is called <span class="tex-font-style-it">powerful</span> if it is a power of two or a factorial. In other words, the number $m$ is powerful if there exists a non-negative integer $d$ such that $m=2^d$ or $m=d!$, where $d!=1\cdot 2\cdot \ldots \cdot d$ (in particular, $0! = 1$). For example $1$, $4$, and $6$ are powerful numbers, because $1=1!$, $4=2^2$, and $6=3!$ but $7$, $10$, or $18$ are not.</p><p>You are given a positive integer $n$. Find the minimum number $k$ such that $n$ can be represented as the sum of $k$ <span class="tex-font-style-bf">distinct</span> powerful numbers, or say that there is no such $k$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>A test case consists of only one line, containing one integer $n$ ($1\le n\le 10^{12}$).</p></div><div class="output-specification"><p>For each test case print the answer on a separate line.</p><p>If $n$ can not be represented as the sum of <span class="tex-font-style-bf">distinct</span> powerful numbers, print $-1$.</p><p>Otherwise, print a single positive integer &nbsp;— the minimum possible value of $k$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>A test case consists of only one line, containing one integer $n$ ($1\le n\le 10^{12}$).</p>

## Output

<p>For each test case print the answer on a separate line.</p><p>If $n$ can not be represented as the sum of <span class="tex-font-style-bf">distinct</span> powerful numbers, print $-1$.</p><p>Otherwise, print a single positive integer &nbsp;— the minimum possible value of $k$.</p>





```input1
4
7
11
240
17179869184
```




```output1
2
3
4
1
```



## Note

<p>In the first test case, $7$ can be represented as $7=1+6$, where $1$ and $6$ are powerful numbers. Because $7$ is not a powerful number, we know that the minimum possible value of $k$ in this case is $k=2$.</p><p>In the second test case, a possible way to represent $11$ as the sum of three powerful numbers is $11=1+4+6$. We can show that there is no way to represent $11$ as the sum of two or less powerful numbers. </p><p>In the third test case, $240$ can be represented as $240=24+32+64+120$. Observe that $240=120+120$ is not a valid representation, because the powerful numbers have to be <span class="tex-font-style-bf">distinct</span>. </p><p>In the fourth test case, $17179869184=2^{34}$, so $17179869184$ is a powerful number and the minimum $k$ in this case is $k=1$.</p>
