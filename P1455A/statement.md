## Description

<div><p>Let's define a function $f(x)$ ($x$ is a positive integer) as follows: write all digits of the decimal representation of $x$ backwards, then get rid of the leading zeroes. For example, $f(321) = 123$, $f(120) = 21$, $f(1000000) = 1$, $f(111) = 111$.</p><p>Let's define another function $g(x) = \dfrac{x}{f(f(x))}$ ($x$ is a positive integer as well).</p><p>Your task is the following: for the given positive integer $n$, calculate the number of different values of $g(x)$ among all numbers $x$ such that $1 \le x \le n$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n &lt; 10^{100}$). This integer is given without leading zeroes.</p></div><div class="output-specification"><p>For each test case, print one integer — the number of different values of the function $g(x)$, if $x$ can be any integer from $[1, n]$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n &lt; 10^{100}$). This integer is given without leading zeroes.</p>

## Output

<p>For each test case, print one integer — the number of different values of the function $g(x)$, if $x$ can be any integer from $[1, n]$.</p>





```input1
5
4
37
998244353
1000000007
12345678901337426966631415
```




```output1
1
2
9
10
26
```



## Note

<p>Explanations for the two first test cases of the example:</p><ol> <li> if $n = 4$, then for every integer $x$ such that $1 \le x \le n$, $\dfrac{x}{f(f(x))} = 1$; </li><li> if $n = 37$, then for some integers $x$ such that $1 \le x \le n$, $\dfrac{x}{f(f(x))} = 1$ (for example, if $x = 23$, $f(f(x)) = 23$,$\dfrac{x}{f(f(x))} = 1$); and for other values of $x$, $\dfrac{x}{f(f(x))} = 10$ (for example, if $x = 30$, $f(f(x)) = 3$, $\dfrac{x}{f(f(x))} = 10$). So, there are two different values of $g(x)$. </li></ol>
