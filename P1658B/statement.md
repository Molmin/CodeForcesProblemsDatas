## Description

<div><p>Marin wants you to count number of permutations that are <span class="tex-font-style-it">beautiful</span>. A <span class="tex-font-style-it">beautiful</span> permutation of length $n$ is a permutation that has the following property: $$ \gcd (1 \cdot p_1, \, 2 \cdot p_2, \, \dots, \, n \cdot p_n) &gt; 1, $$ where $\gcd$ is the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a>.</p><p>A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3, 4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 10^3$).</p></div><div class="output-specification"><p>For each test case, print one integer — number of <span class="tex-font-style-it">beautiful</span> permutations. Because the answer can be very big, please print the answer modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^3$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 10^3$).</p>

## Output

<p>For each test case, print one integer — number of <span class="tex-font-style-it">beautiful</span> permutations. Because the answer can be very big, please print the answer modulo $998\,244\,353$.</p>





```input1
7
1
2
3
4
5
6
1000
```




```output1
0
1
0
4
0
36
665702330
```



## Note

<p>In first test case, we only have one permutation which is $[1]$ but it is not beautiful because $\gcd(1 \cdot 1) = 1$.</p><p>In second test case, we only have one beautiful permutation which is $[2, 1]$ because $\gcd(1 \cdot 2, 2 \cdot 1) = 2$. </p>
