## Description

<div><p>Tokitsukaze has a sequence $a$ of length $n$. For each operation, she selects two numbers $a_i$ and $a_j$ ($i \ne j$; $1 \leq i,j \leq n$). </p><ul> <li> If $a_i = a_j$, change one of them to $0$. </li><li> Otherwise change both of them to $\min(a_i, a_j)$. </li></ul><p>Tokitsukaze wants to know the minimum number of operations to change all numbers in the sequence to $0$. It can be proved that the answer always exists.</p></div><div class="input-specification"><p>The first line contains a single positive integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains a single integer $n$ ($2 \leq n \leq 100$)&nbsp;— the length of the sequence $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 100$)&nbsp;— the sequence $a$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the minimum number of operations to change all numbers in the sequence to $0$.</p></div>

## Input

<p>The first line contains a single positive integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains a single integer $n$ ($2 \leq n \leq 100$)&nbsp;— the length of the sequence $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 100$)&nbsp;— the sequence $a$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the minimum number of operations to change all numbers in the sequence to $0$.</p>





```input1
3
3
1 2 3
3
1 2 2
3
1 2 0
```




```output1
4
3
2
```



## Note

<p>In the first test case, one of the possible ways to change all numbers in the sequence to $0$:</p><p>In the $1$-st operation, $a_1 &lt; a_2$, after the operation, $a_2 = a_1 = 1$. Now the sequence $a$ is $[1,1,3]$.</p><p>In the $2$-nd operation, $a_1 = a_2 = 1$, after the operation, $a_1 = 0$. Now the sequence $a$ is $[0,1,3]$.</p><p>In the $3$-rd operation, $a_1 &lt; a_2$, after the operation, $a_2 = 0$. Now the sequence $a$ is $[0,0,3]$.</p><p>In the $4$-th operation, $a_2 &lt; a_3$, after the operation, $a_3 = 0$. Now the sequence $a$ is $[0,0,0]$.</p><p>So the minimum number of operations is $4$.</p>
