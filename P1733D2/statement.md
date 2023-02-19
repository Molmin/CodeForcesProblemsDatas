## Description

<div><p><span class="tex-font-style-bf">This is the hard version of this problem. In this version, $n \le 5000$ holds, and this version has no restriction between $x$ and $y$. You can make hacks only if both versions of the problem are solved.</span></p><p>You are given two binary strings $a$ and $b$, both of length $n$. You can do the following operation any number of times (possibly zero). </p><ul> <li> Select two indices $l$ and $r$ ($l &lt; r$). </li><li> Change $a_l$ to $(1 - a_l)$, and $a_r$ to $(1 - a_r)$. </li><li> If $l + 1 = r$, the cost of the operation is $x$. Otherwise, the cost is $y$. </li></ul><p>You have to find the minimum cost needed to make $a$ equal to $b$ or say there is no way to do so.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of three lines. The first line of each test case contains three integers $n$, $x$, and $y$ ($5 \le n \le 5000$, $1 \le x, y \le 10^9$)&nbsp;— the length of the strings, and the costs per operation.</p><p>The second line of each test case contains the string $a$ of length $n$. The string only consists of digits $0$ and $1$.</p><p>The third line of each test case contains the string $b$ of length $n$. The string only consists of digits $0$ and $1$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $5000$.</p></div><div class="output-specification"><p>For each test case, if there is no way to make $a$ equal to $b$, print $-1$. Otherwise, print the minimum cost needed to make $a$ equal to $b$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of three lines. The first line of each test case contains three integers $n$, $x$, and $y$ ($5 \le n \le 5000$, $1 \le x, y \le 10^9$)&nbsp;— the length of the strings, and the costs per operation.</p><p>The second line of each test case contains the string $a$ of length $n$. The string only consists of digits $0$ and $1$.</p><p>The third line of each test case contains the string $b$ of length $n$. The string only consists of digits $0$ and $1$.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $5000$.</p>

## Output

<p>For each test case, if there is no way to make $a$ equal to $b$, print $-1$. Otherwise, print the minimum cost needed to make $a$ equal to $b$.</p>





```input1|2,3,4,8,9,10,14,15,16
6
5 8 9
01001
00101
6 2 11
000001
100000
5 7 2
01000
11011
7 8 3
0111001
0100001
6 3 4
010001
101000
5 10 1
01100
01100
```




```output1
8
10
-1
6
7
0
```



## Note

<p>In the first test case, selecting indices $2$ and $3$ costs $8$, which is the minimum.</p><p>In the second test case, we can perform the following operations. </p><ul> <li> Select indices $1$ and $2$. It costs $2$, and $a$ is <span class="tex-font-style-tt">110001</span> now. </li><li> Select indices $2$ and $3$. It costs $2$, and $a$ is <span class="tex-font-style-tt">101001</span> now. </li><li> Select indices $3$ and $4$. It costs $2$, and $a$ is <span class="tex-font-style-tt">100101</span> now. </li><li> Select indices $4$ and $5$. It costs $2$, and $a$ is <span class="tex-font-style-tt">100011</span> now. </li><li> Select indices $5$ and $6$. It costs $2$, and $a$ is <span class="tex-font-style-tt">100000</span> now. </li></ul><p>The total cost is $10$.</p><p>In the third test case, we cannot make $a$ equal to $b$ using any number of operations.</p><p>In the fourth test case, we can perform the following operations. </p><ul> <li> Select indices $3$ and $6$. It costs $3$, and $a$ is <span class="tex-font-style-tt">0101011</span> now. </li><li> Select indices $4$ and $6$. It costs $3$, and $a$ is <span class="tex-font-style-tt">0100001</span> now. </li></ul><p>The total cost is $6$.</p><p>In the fifth test case, we can perform the following operations. </p><ul> <li> Select indices $1$ and $6$. It costs $4$, and $a$ is <span class="tex-font-style-tt">110000</span> now. </li><li> Select indices $2$ and $3$. It costs $3$, and $a$ is <span class="tex-font-style-tt">101000</span> now. </li></ul><p>The total cost is $7$.</p><p>In the sixth test case, we don't have to perform any operation.</p>
