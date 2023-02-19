## Description

<div><p><span class="tex-font-style-it">During their training for the ICPC competitions, team "Jee You See" stumbled upon a very basic counting problem. After many "Wrong answer" verdicts, they finally decided to give up and <span class="tex-font-style-striked">destroy</span> turn-off the PC. Now they want your help in up-solving the problem.</span></p><p>You are given 4 integers $n$, $l$, $r$, and $z$. Count the number of arrays $a$ of length $n$ containing non-negative integers such that:</p><ul> <li> $l\le a_1+a_2+\ldots+a_n\le r$, and </li><li> $a_1\oplus a_2 \oplus \ldots\oplus a_n=z$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> operation. </li></ul><p>Since the answer can be large, print it modulo $10^9+7$.</p></div><div class="input-specification"><p>The only line contains four integers $n$, $l$, $r$, $z$ ($1 \le n \le 1000$, $1\le l\le r\le 10^{18}$, $1\le z\le 10^{18}$).</p></div><div class="output-specification"><p>Print the number of arrays $a$ satisfying all requirements modulo $10^9+7$.</p></div>

## Input

<p>The only line contains four integers $n$, $l$, $r$, $z$ ($1 \le n \le 1000$, $1\le l\le r\le 10^{18}$, $1\le z\le 10^{18}$).</p>

## Output

<p>Print the number of arrays $a$ satisfying all requirements modulo $10^9+7$.</p>





```input1
3 1 5 1
```




```input2
4 1 3 2
```




```input3
2 1 100000 15629
```




```input4
100 56 89 66
```




```output1
13
```




```output2
4
```




```output3
49152
```




```output4
981727503
```



## Note

<p>The following arrays satisfy the conditions for the first sample:</p><ul> <li> $[1, 0, 0]$; </li><li> $[0, 1, 0]$; </li><li> $[3, 2, 0]$; </li><li> $[2, 3, 0]$; </li><li> $[0, 0, 1]$; </li><li> $[1, 1, 1]$; </li><li> $[2, 2, 1]$; </li><li> $[3, 0, 2]$; </li><li> $[2, 1, 2]$; </li><li> $[1, 2, 2]$; </li><li> $[0, 3, 2]$; </li><li> $[2, 0, 3]$; </li><li> $[0, 2, 3]$. </li></ul><p>The following arrays satisfy the conditions for the second sample:</p><ul> <li> $[2, 0, 0, 0]$; </li><li> $[0, 2, 0, 0]$; </li><li> $[0, 0, 2, 0]$; </li><li> $[0, 0, 0, 2]$. </li></ul>
