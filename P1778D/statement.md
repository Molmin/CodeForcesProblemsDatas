## Description

<div><p>You are given two binary strings $a$ and $b$ of length $n$. In each move, the string $a$ is modified in the following way.</p><ul> <li> An index $i$ ($1 \leq i \leq n$) is chosen uniformly at random. The character $a_i$ will be flipped. That is, if $a_i$ is $0$, it becomes $1$, and if $a_i$ is $1$, it becomes $0$. </li></ul><p>What is the expected number of moves required to make both strings equal <span class="tex-font-style-bf">for the first time</span>?</p><p>A binary string is a string, in which the character is either $\tt{0}$ or $\tt{1}$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the length of the strings.</p><p>The second line of each test case contains the binary string $a$ of length $n$.</p><p>The third line of each test case contains the binary string $b$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output a single line containing the expected number of moves modulo $998\,244\,353$.</p><p>Formally, let $M = 998\,244\,353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^5$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 10^6$)&nbsp;— the length of the strings.</p><p>The second line of each test case contains the binary string $a$ of length $n$.</p><p>The third line of each test case contains the binary string $b$ of length $n$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case, output a single line containing the expected number of moves modulo $998\,244\,353$.</p><p>Formally, let $M = 998\,244\,353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p>





```input1|2,3,4,8,9,10
4
1
0
1
2
00
00
4
1000
1110
5
01001
10111
```




```output1
1
0
665496254
665496277
```



## Note

<p>In the first test case, index $1$ is chosen randomly and $a_1$ is flipped. After the move, the strings $a$ and $b$ are equal. The expected number of moves is $1$.</p><p>The strings $a$ and $b$ are already equal in the second test case. So, the expected number of moves is $0$.</p><p>The expected number of moves for the third and fourth test cases are $\frac{56}{3}$ and $\frac{125}{3}$ respectively.</p>
