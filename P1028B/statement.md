## Description

<div><p>Let $s(x)$ be sum of digits in decimal representation of positive integer $x$. Given two integers $n$ and $m$, find some positive integers $a$ and $b$ such that </p><ul> <li> $s(a) \ge n$, </li><li> $s(b) \ge n$, </li><li> $s(a + b) \le m$. </li></ul></div><div class="input-specification"><p>The only line of input contain two integers $n$ and $m$ ($1 \le n, m \le 1129$).</p></div><div class="output-specification"><p>Print two lines, one for decimal representation of $a$ and one for decimal representation of $b$. Both numbers must not contain leading zeros and must have length no more than $2230$.</p></div>

## Input

<p>The only line of input contain two integers $n$ and $m$ ($1 \le n, m \le 1129$).</p>

## Output

<p>Print two lines, one for decimal representation of $a$ and one for decimal representation of $b$. Both numbers must not contain leading zeros and must have length no more than $2230$.</p>





```input1
6 5

```




```input2
8 16

```




```output1
6 
7

```




```output2
35 
53

```



## Note

<p>In the first sample, we have $n = 6$ and $m = 5$. One valid solution is $a = 6$, $b = 7$. Indeed, we have $s(a) = 6 \ge n$ and $s(b) = 7 \ge n$, and also $s(a + b) = s(13) = 4 \le m$.</p>
