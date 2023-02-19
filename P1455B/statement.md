## Description

<div><p>You are standing on the $\mathit{OX}$-axis at point $0$ and you want to move to an integer point $x &gt; 0$.</p><p>You can make several jumps. Suppose you're currently at point $y$ ($y$ may be negative) and jump for the $k$-th time. You can: </p><ul> <li> either jump to the point $y + k$ </li><li> or jump to the point $y - 1$. </li></ul><p>What is the minimum number of jumps you need to reach the point $x$?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains the single integer $x$ ($1 \le x \le 10^6$)&nbsp;— the destination point.</p></div><div class="output-specification"><p>For each test case, print the single integer&nbsp;— the minimum number of jumps to reach $x$. It can be proved that we can reach any integer point $x$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains the single integer $x$ ($1 \le x \le 10^6$)&nbsp;— the destination point.</p>

## Output

<p>For each test case, print the single integer&nbsp;— the minimum number of jumps to reach $x$. It can be proved that we can reach any integer point $x$.</p>





```input1
5
1
2
3
4
5
```




```output1
1
3
2
3
4
```



## Note

<p>In the first test case $x = 1$, so you need only one jump: the $1$-st jump from $0$ to $0 + 1 = 1$.</p><p>In the second test case $x = 2$. You need at least three jumps: </p><ul> <li> the $1$-st jump from $0$ to $0 + 1 = 1$; </li><li> the $2$-nd jump from $1$ to $1 + 2 = 3$; </li><li> the $3$-rd jump from $3$ to $3 - 1 = 2$; </li></ul><p>Two jumps are not enough because these are the only possible variants: </p><ul> <li> the $1$-st jump as $-1$ and the $2$-nd one as $-1$&nbsp;— you'll reach $0 -1 -1 =-2$; </li><li> the $1$-st jump as $-1$ and the $2$-nd one as $+2$&nbsp;— you'll reach $0 -1 +2 = 1$; </li><li> the $1$-st jump as $+1$ and the $2$-nd one as $-1$&nbsp;— you'll reach $0 +1 -1 = 0$; </li><li> the $1$-st jump as $+1$ and the $2$-nd one as $+2$&nbsp;— you'll reach $0 +1 +2 = 3$; </li></ul><p>In the third test case, you need two jumps: the $1$-st one as $+1$ and the $2$-nd one as $+2$, so $0 + 1 + 2 = 3$.</p><p>In the fourth test case, you need three jumps: the $1$-st one as $-1$, the $2$-nd one as $+2$ and the $3$-rd one as $+3$, so $0 - 1 + 2 + 3 = 4$.</p>
