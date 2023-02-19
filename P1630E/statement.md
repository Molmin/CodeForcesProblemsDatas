## Description

<div><p>Given a cyclic array $a$ of size $n$, where $a_i$ is the value of $a$ in the $i$-th position, <span class="tex-font-style-bf">there may be repeated values</span>. Let us define that a permutation of $a$ is equal to another permutation of $a$ if and only if their values are the same for each position $i$ or we can transform them to each other by performing some cyclic rotation. Let us define for a cyclic array $b$ its number of components as the number of connected components in a graph, where the vertices are the positions of $b$ and we add an edge between each pair of adjacent positions of $b$ with equal values (note that in a cyclic array the first and last position are also adjacents).</p><p>Find the expected value of components of a permutation of $a$ if we select it equiprobably over the set of all the different permutations of $a$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^6$) — the size of the cyclic array $a$.</p><p>The second line of each test case contains $n$ integers, the $i$-th of them is the value $a_i$ ($1 \le a_i \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p><p>It is guaranteed that the total number of different permutations of $a$ is not divisible by $M$</p></div><div class="output-specification"><p>For each test case print a single integer — the expected value of components of a permutation of $a$ if we select it equiprobably over the set of all the different permutations of $a$ modulo $998\,244\,353$. </p><p>Formally, let $M = 998\,244\,353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^6$) — the size of the cyclic array $a$.</p><p>The second line of each test case contains $n$ integers, the $i$-th of them is the value $a_i$ ($1 \le a_i \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p><p>It is guaranteed that the total number of different permutations of $a$ is not divisible by $M$</p>

## Output

<p>For each test case print a single integer — the expected value of components of a permutation of $a$ if we select it equiprobably over the set of all the different permutations of $a$ modulo $998\,244\,353$. </p><p>Formally, let $M = 998\,244\,353$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p>





```input1|2,3,6,7,10,11
5
4
1 1 1 1
4
1 1 2 1
4
1 2 1 2
5
4 3 2 5 1
12
1 3 2 3 2 1 3 3 1 3 3 2
```




```output1
1
2
3
5
358642921
```



## Note

<p>In the first test case there is only $1$ different permutation of $a$:</p><ul> <li> $[1, 1, 1, 1]$ has $1$ component. </li><li> Therefore the expected value of components is $\frac{1}{1} = 1$ </li></ul><p>In the second test case there are $4$ ways to permute the cyclic array $a$, but there is only $1$ different permutation of $a$:</p><ul> <li> $[1, 1, 1, 2]$, $[1, 1, 2, 1]$, $[1, 2, 1, 1]$ and $[2, 1, 1, 1]$ are the same permutation and have $2$ components. </li><li> Therefore the expected value of components is $\frac{2}{1} = 2$ </li></ul><p>In the third test case there are $6$ ways to permute the cyclic array $a$, but there are only $2$ different permutations of $a$:</p><ul> <li> $[1, 1, 2, 2]$, $[2, 1, 1, 2]$, $[2, 2, 1, 1]$ and $[1, 2, 2, 1]$ are the same permutation and have $2$ components. </li><li> $[1, 2, 1, 2]$ and $[2, 1, 2, 1]$ are the same permutation and have $4$ components. </li><li> Therefore the expected value of components is $\frac{2+4}{2} = \frac{6}{2} = 3$ </li></ul><p>In the fourth test case there are $120$ ways to permute the cyclic array $a$, but there are only $24$ different permutations of $a$:</p><ul> <li> Any permutation of $a$ has $5$ components. </li><li> Therefore the expected value of components is $\frac{24\cdot 5}{24} = \frac{120}{24} = 5$ </li></ul>
