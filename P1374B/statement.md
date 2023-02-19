## Description

<div><p>You are given an integer $n$. In one move, you can either multiply $n$ by two or divide $n$ by $6$ (if it is divisible by $6$ without the remainder).</p><p>Your task is to find the minimum number of moves needed to obtain $1$ from $n$ or determine if it's impossible to do that.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow. </p><p>The only line of the test case contains one integer $n$ ($1 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print the answer — the minimum number of moves needed to obtain $1$ from $n$ if it's possible to do that or <span class="tex-font-style-tt">-1</span> if it's impossible to obtain $1$ from $n$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow. </p><p>The only line of the test case contains one integer $n$ ($1 \le n \le 10^9$).</p>

## Output

<p>For each test case, print the answer — the minimum number of moves needed to obtain $1$ from $n$ if it's possible to do that or <span class="tex-font-style-tt">-1</span> if it's impossible to obtain $1$ from $n$.</p>





```input1
7
1
2
3
12
12345
15116544
387420489
```




```output1
0
-1
2
-1
-1
12
36
```



## Note

<p>Consider the sixth test case of the example. The answer can be obtained by the following sequence of moves from the given integer $15116544$:</p><ol> <li> Divide by $6$ and get $2519424$; </li><li> divide by $6$ and get $419904$; </li><li> divide by $6$ and get $69984$; </li><li> divide by $6$ and get $11664$; </li><li> multiply by $2$ and get $23328$; </li><li> divide by $6$ and get $3888$; </li><li> divide by $6$ and get $648$; </li><li> divide by $6$ and get $108$; </li><li> multiply by $2$ and get $216$; </li><li> divide by $6$ and get $36$; </li><li> divide by $6$ and get $6$; </li><li> divide by $6$ and get $1$. </li></ol>
