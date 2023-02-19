## Description

<div><p>You are given a sequence $a_1, a_2, \ldots, a_n$. Each element of $a$ is $1$ or $2$.</p><p>Find out if an integer $k$ exists so that the following conditions are met. </p><ul> <li> $1 \leq k \leq n-1$, and </li><li> $a_1 \cdot a_2 \cdot \ldots \cdot a_k = a_{k+1} \cdot a_{k+2} \cdot \ldots \cdot a_n$. </li></ul><p>If there exist multiple $k$ that satisfy the given condition, print the smallest.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 1000$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 2$).</p></div><div class="output-specification"><p>For each test case, if there is no such $k$, print $-1$.</p><p>Otherwise, print the smallest possible $k$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 1000$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 2$).</p>

## Output

<p>For each test case, if there is no such $k$, print $-1$.</p><p>Otherwise, print the smallest possible $k$.</p>





```input1|2,3,6,7
3
6
2 2 1 2 1 2
3
1 2 1
4
1 1 1 1
```




```output1
2
-1
1
```



## Note

<p>For the first test case, $k=2$ satisfies the condition since $a_1 \cdot a_2 = a_3 \cdot a_4 \cdot a_5 \cdot a_6 = 4$. $k=3$ also satisfies the given condition, but the smallest should be printed.</p><p>For the second test case, there is no $k$ that satisfies $a_1 \cdot a_2 \cdot \ldots \cdot a_k = a_{k+1} \cdot a_{k+2} \cdot \ldots \cdot a_n$</p><p>For the third test case, $k=1$, $2$, and $3$ satisfy the given condition, so the answer is $1$.</p>
