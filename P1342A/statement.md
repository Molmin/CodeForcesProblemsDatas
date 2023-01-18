## Description

<div><p>You are given two integers $x$ and $y$. You can perform two types of operations: </p><ol> <li> Pay $a$ dollars and increase or decrease any of these integers by $1$. For example, if $x = 0$ and $y = 7$ there are four possible outcomes after this operation: <ul> <li> $x = 0$, $y = 6$; </li><li> $x = 0$, $y = 8$; </li><li> $x = -1$, $y = 7$; </li><li> $x = 1$, $y = 7$. </li></ul><p> </p></li><li> Pay $b$ dollars and increase or decrease both integers by $1$. For example, if $x = 0$ and $y = 7$ there are two possible outcomes after this operation: <ul> <li> $x = -1$, $y = 6$; </li><li> $x = 1$, $y = 8$. </li></ul> </li></ol><p>Your goal is to make both given integers equal zero simultaneously, i.e. $x = y = 0$. There are no other requirements. In particular, it is possible to move from $x=1$, $y=0$ to $x=y=0$.</p><p>Calculate the minimum amount of dollars you have to spend on it.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 100$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains two integers $x$ and $y$ ($0 \le x, y \le 10^9$).</p><p>The second line of each test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the minimum amount of dollars you have to spend.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 100$)&nbsp;— the number of testcases.</p><p>The first line of each test case contains two integers $x$ and $y$ ($0 \le x, y \le 10^9$).</p><p>The second line of each test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p>

## Output

<p>For each test case print one integer&nbsp;— the minimum amount of dollars you have to spend.</p>





```input1
2
1 3
391 555
0 0
9 4
```




```output1
1337
0
```



## Note

<p>In the first test case you can perform the following sequence of operations: first, second, first. This way you spend $391 + 555 + 391 = 1337$ dollars.</p><p>In the second test case both integers are equal to zero initially, so you dont' have to spend money.</p>
