## Description

<div><p>You are given three integers $a$, $b$ and $c$.</p><p>Find two positive integers $x$ and $y$ ($x &gt; 0$, $y &gt; 0$) such that: </p><ul> <li> the decimal representation of $x$ without leading zeroes consists of $a$ digits; </li><li> the decimal representation of $y$ without leading zeroes consists of $b$ digits; </li><li> the decimal representation of $gcd(x, y)$ without leading zeroes consists of $c$ digits. </li></ul><p>$gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$.</p><p>Output $x$ and $y$. If there are multiple answers, output any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 285$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains three integers $a$, $b$ and $c$ ($1 \le a, b \le 9$, $1 \le c \le min(a, b)$)&nbsp;— the required lengths of the numbers.</p><p>It can be shown that the answer exists for all testcases under the given constraints.</p><p>Additional constraint on the input: all testcases are different.</p></div><div class="output-specification"><p>For each testcase print two positive integers&nbsp;— $x$ and $y$ ($x &gt; 0$, $y &gt; 0$) such that </p><ul> <li> the decimal representation of $x$ without leading zeroes consists of $a$ digits; </li><li> the decimal representation of $y$ without leading zeroes consists of $b$ digits; </li><li> the decimal representation of $gcd(x, y)$ without leading zeroes consists of $c$ digits. </li></ul></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 285$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains three integers $a$, $b$ and $c$ ($1 \le a, b \le 9$, $1 \le c \le min(a, b)$)&nbsp;— the required lengths of the numbers.</p><p>It can be shown that the answer exists for all testcases under the given constraints.</p><p>Additional constraint on the input: all testcases are different.</p>

## Output

<p>For each testcase print two positive integers&nbsp;— $x$ and $y$ ($x &gt; 0$, $y &gt; 0$) such that </p><ul> <li> the decimal representation of $x$ without leading zeroes consists of $a$ digits; </li><li> the decimal representation of $y$ without leading zeroes consists of $b$ digits; </li><li> the decimal representation of $gcd(x, y)$ without leading zeroes consists of $c$ digits. </li></ul>





```input1
4
2 3 1
2 2 2
6 6 2
1 1 1
```




```output1
11 492
13 26
140133 160776
1 1
```



## Note

<p>In the example: </p><ol> <li> $gcd(11, 492) = 1$ </li><li> $gcd(13, 26) = 13$ </li><li> $gcd(140133, 160776) = 21$ </li><li> $gcd(1, 1) = 1$ </li></ol>
