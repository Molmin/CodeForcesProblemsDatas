## Description

<div><p>Ridbit starts with an integer $n$.</p><p>In one move, he can perform one of the following operations: </p><ul> <li> divide $n$ by one of its <span class="tex-font-style-bf">proper</span> divisors, or </li><li> subtract $1$ from $n$ if $n$ is greater than $1$. </li></ul><p>A proper divisor is a divisor of a number, excluding itself. For example, $1$, $2$, $4$, $5$, and $10$ are proper divisors of $20$, but $20$ itself is not.</p><p>What is the minimum number of moves Ridbit is required to make to reduce $n$ to $1$?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \leq n \leq 10^9$).</p></div><div class="output-specification"><p>For each test case, output the minimum number of moves required to reduce $n$ to $1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($1 \leq n \leq 10^9$).</p>

## Output

<p>For each test case, output the minimum number of moves required to reduce $n$ to $1$.</p>





```input1
6
1
2
3
4
6
9
```




```output1
0
1
2
2
2
3
```



## Note

<p>For the test cases in the example, $n$ may be reduced to $1$ using the following operations in sequence</p><p>$1$</p><p>$2 \xrightarrow{} 1$</p><p>$3 \xrightarrow{} 2 \xrightarrow{} 1$</p><p>$4 \xrightarrow{} 2 \xrightarrow{} 1$</p><p>$6 \xrightarrow{} 2 \xrightarrow{} 1$</p><p>$9 \xrightarrow{} 3 \xrightarrow{} 2\xrightarrow{} 1$</p>
