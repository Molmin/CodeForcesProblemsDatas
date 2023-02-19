## Description

<div><p>You are given an array $a$ consisting of $n$ integers $a_1, a_2, \ldots, a_n$. Friends asked you to make the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of all numbers in the array equal to $1$. In one operation, you can do the following:</p><ul><li> Select an arbitrary index in the array $1 \leq i \leq n$;</li><li> Make $a_i = \gcd(a_i, i)$, where $\gcd(x, y)$ denotes the GCD of integers $x$ and $y$. The cost of such an operation is $n - i + 1$.</li></ul><p>You need to find the minimum total cost of operations we need to perform so that the GCD of the all array numbers becomes equal to $1$.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 5\,000$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 20$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — the elements of the array.</p></div><div class="output-specification"><p>For each test case, output a single integer — the minimum total cost of operations that will need to be performed so that the GCD of all numbers in the array becomes equal to $1$.</p><p>We can show that it's always possible to do so.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 5\,000$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 20$) — the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — the elements of the array.</p>

## Output

<p>For each test case, output a single integer — the minimum total cost of operations that will need to be performed so that the GCD of all numbers in the array becomes equal to $1$.</p><p>We can show that it's always possible to do so.</p>





```input1|2,3,6,7,10,11,14,15,18,19
9
1
1
1
2
2
2 4
3
3 6 9
4
5 10 15 20
5
120 60 80 40 80
6
150 90 180 120 60 30
6
2 4 6 9 12 18
6
30 60 90 120 125 125
```




```output1
0
1
2
2
1
3
3
0
1
```



## Note

<p>In the first test case, the GCD of the entire array is already equal to $1$, so there is no need to perform operations.</p><p>In the second test case, select $i = 1$. After this operation, $a_1 = \gcd(2, 1) = 1$. The cost of this operation is $1$.</p><p>In the third test case, you can select $i = 1$, after that the array $a$ will be equal to $[1, 4]$. The GCD of this array is $1$, and the total cost is $2$.</p><p>In the fourth test case, you can select $i = 2$, after that the array $a$ will be equal to $[3, 2, 9]$. The GCD of this array is $1$, and the total cost is $2$.</p><p>In the sixth test case, you can select $i = 4$ and $i = 5$, after that the array $a$ will be equal to $[120, 60, 80, 4, 5]$. The GCD of this array is $1$, and the total cost is $3$.</p>
