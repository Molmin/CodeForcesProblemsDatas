## Description

<div><p>You are given three integers $n$, $l$, and $r$. You need to construct an array $a_1,a_2,\dots,a_n$ ($l\le a_i\le r$) such that $\gcd(i,a_i)$ are all distinct or report there's no solution.</p><p>Here $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains three integers $n$, $l$, $r$ ($1 \le n \le 10^5$, $1\le l\le r\le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, if there is no solution, print "<span class="tex-font-style-tt">NO</span>" (without quotes). You can print letters in any case (upper or lower).</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without quotes). In the next line, print $n$ integers $a_1,a_2,\ldots,a_n$&nbsp;— the array you construct.</p><p>If there are multiple solutions, you may output any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line contains three integers $n$, $l$, $r$ ($1 \le n \le 10^5$, $1\le l\le r\le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, if there is no solution, print "<span class="tex-font-style-tt">NO</span>" (without quotes). You can print letters in any case (upper or lower).</p><p>Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without quotes). In the next line, print $n$ integers $a_1,a_2,\ldots,a_n$&nbsp;— the array you construct.</p><p>If there are multiple solutions, you may output any.</p>





```input1
4
5 1 5
9 1000 2000
10 30 35
1 1000000000 1000000000
```




```output1
YES
1 2 3 4 5
YES
1145 1926 1440 1220 1230 1350 1001 1000 1233
NO
YES
1000000000
```



## Note

<p>In the first test case, $\gcd(1,a_1),\gcd(2,a_2),\ldots,\gcd(5,a_5)$ are equal to $1$, $2$, $3$, $4$, $5$, respectively.</p>
