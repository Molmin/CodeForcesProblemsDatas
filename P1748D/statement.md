## Description

<div><p>You are given three integers $a$, $b$, and $d$. Your task is to find any integer $x$ which satisfies all of the following conditions, or determine that no such integers exist:</p><ul> <li> $0 \le x \lt 2^{60}$; </li><li> $a|x$ is divisible by $d$; </li><li> $b|x$ is divisible by $d$. </li></ul><p>Here, $|$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR operation</a>.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line of input contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. </p><p>Each test case consists of one line, containing three integers $a$, $b$, and $d$ ($1 \le a,b,d \lt 2^{30}$).</p></div><div class="output-specification"><p>For each test case print one integer. If there exists an integer $x$ which satisfies all of the conditions from the statement, print $x$. Otherwise, print $-1$.</p><p>If there are multiple solutions, you may print <span class="tex-font-style-bf">any</span> of them. </p></div>

## Input

<p>Each test contains multiple test cases. The first line of input contains one integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. </p><p>Each test case consists of one line, containing three integers $a$, $b$, and $d$ ($1 \le a,b,d \lt 2^{30}$).</p>

## Output

<p>For each test case print one integer. If there exists an integer $x$ which satisfies all of the conditions from the statement, print $x$. Otherwise, print $-1$.</p><p>If there are multiple solutions, you may print <span class="tex-font-style-bf">any</span> of them. </p>





```input1|2,4,6,8
8
12 39 5
6 8 14
100 200 200
3 4 6
2 2 2
18 27 3
420 666 69
987654321 123456789 999999999
```




```output1
18
14
-1
-1
0
11
25599
184470016815529983
```



## Note

<p>In the first test case, $x=18$ is one of the possible solutions, since $39|18=55$ and $12|18=30$, both of which are multiples of $d=5$.</p><p>In the second test case, $x=14$ is one of the possible solutions, since $8|14=6|14=14$, which is a multiple of $d=14$.</p><p>In the third and fourth test cases, we can show that there are no solutions.</p>
