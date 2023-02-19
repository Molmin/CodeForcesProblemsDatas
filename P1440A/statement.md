## Description

<div><p>You are given four integers $n$, $c_0$, $c_1$ and $h$ and a binary string $s$ of length $n$.</p><p>A binary string is a string consisting of characters $0$ and $1$.</p><p>You can change any character of the string $s$ (the string should be still binary after the change). You should pay $h$ coins for each change.</p><p>After some changes (possibly zero) you want to buy the string. To buy the string you should buy all its characters. To buy the character $0$ you should pay $c_0$ coins, to buy the character $1$ you should pay $c_1$ coins.</p><p>Find the minimum number of coins needed to buy the string.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10$)&nbsp;— the number of test cases. Next $2t$ lines contain descriptions of test cases.</p><p>The first line of the description of each test case contains four integers $n$, $c_{0}$, $c_{1}$, $h$ ($1 \leq n, c_{0}, c_{1}, h \leq 1000$).</p><p>The second line of the description of each test case contains the binary string $s$ of length $n$.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the minimum number of coins needed to buy the string.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10$)&nbsp;— the number of test cases. Next $2t$ lines contain descriptions of test cases.</p><p>The first line of the description of each test case contains four integers $n$, $c_{0}$, $c_{1}$, $h$ ($1 \leq n, c_{0}, c_{1}, h \leq 1000$).</p><p>The second line of the description of each test case contains the binary string $s$ of length $n$.</p>

## Output

<p>For each test case print a single integer&nbsp;— the minimum number of coins needed to buy the string.</p>





```input1
6
3 1 1 1
100
5 10 100 1
01010
5 10 1 1
11111
5 1 10 1
11111
12 2 1 10
101110110101
2 100 1 10
00
```




```output1
3
52
5
10
16
22
```



## Note

<p>In the first test case, you can buy all characters and pay $3$ coins, because both characters $0$ and $1$ costs $1$ coin.</p><p>In the second test case, you can firstly change $2$-nd and $4$-th symbols of the string from $1$ to $0$ and pay $2$ coins for that. Your string will be $00000$. After that, you can buy the string and pay $5 \cdot 10 = 50$ coins for that. The total number of coins paid will be $2 + 50 = 52$.</p>
