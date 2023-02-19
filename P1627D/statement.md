## Description

<div><p>You have an array $a_1, a_2, \dots, a_n$ consisting of $n$ <span class="tex-font-style-bf">distinct</span> integers. You are allowed to perform the following operation on it:</p><ul> <li> Choose two elements from the array $a_i$ and $a_j$ ($i \ne j$) such that $\gcd(a_i, a_j)$ is not present in the array, and add $\gcd(a_i, a_j)$ to the end of the array. Here $\gcd(x, y)$ denotes <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$. </li></ul><p>Note that the array changes after each operation, and the subsequent operations are performed on the new array.</p><p>What is the <span class="tex-font-style-bf">maximum</span> number of times you can perform the operation on the array?</p></div><div class="input-specification"><p>The first line consists of a single integer $n$ ($2 \le n \le 10^6$).</p><p>The second line consists of $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^6$). All $a_i$ are <span class="tex-font-style-bf">distinct</span>.</p></div><div class="output-specification"><p>Output a single line containing one integer&nbsp;— the maximum number of times the operation can be performed on the given array.</p></div>

## Input

<p>The first line consists of a single integer $n$ ($2 \le n \le 10^6$).</p><p>The second line consists of $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^6$). All $a_i$ are <span class="tex-font-style-bf">distinct</span>.</p>

## Output

<p>Output a single line containing one integer&nbsp;— the maximum number of times the operation can be performed on the given array.</p>





```input1
5
4 20 1 25 30
```




```input2
3
6 10 15
```




```output1
3
```




```output2
4
```



## Note

<p>In the first example, one of the ways to perform maximum number of operations on the array is: </p><ul> <li> Pick $i = 1, j= 5$ and add $\gcd(a_1, a_5) = \gcd(4, 30) = 2$ to the array. </li><li> Pick $i = 2, j= 4$ and add $\gcd(a_2, a_4) = \gcd(20, 25) = 5$ to the array. </li><li> Pick $i = 2, j= 5$ and add $\gcd(a_2, a_5) = \gcd(20, 30) = 10$ to the array. </li></ul><p>It can be proved that there is no way to perform more than $3$ operations on the original array.</p><p>In the second example one can add $3$, then $1$, then $5$, and $2$.</p>
