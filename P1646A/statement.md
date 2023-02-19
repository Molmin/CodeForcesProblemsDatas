## Description

<div><p>Luis has a sequence of $n+1$ integers $a_1, a_2, \ldots, a_{n+1}$. For each $i = 1, 2, \ldots, n+1$ it is guaranteed that $0\leq a_i &lt; n$, or $a_i=n^2$. He has calculated the sum of all the elements of the sequence, and called this value $s$. </p><p>Luis has lost his sequence, but he remembers the values of $n$ and $s$. Can you find the number of elements in the sequence that are equal to $n^2$?</p><p>We can show that the answer is unique under the given constraints.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2\cdot 10^4$). Description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $s$ ($1\le n&lt; 10^6$, $0\le s \le 10^{18}$). It is guaranteed that the value of $s$ is a valid sum for some sequence satisfying the above constraints.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the number of elements in the sequence which are equal to $n^2$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2\cdot 10^4$). Description of the test cases follows.</p><p>The only line of each test case contains two integers $n$ and $s$ ($1\le n&lt; 10^6$, $0\le s \le 10^{18}$). It is guaranteed that the value of $s$ is a valid sum for some sequence satisfying the above constraints.</p>

## Output

<p>For each test case, print one integer&nbsp;— the number of elements in the sequence which are equal to $n^2$.</p>





```input1
4
7 0
1 1
2 12
3 12
```




```output1
0
1
3
1
```



## Note

<p>In the first test case, we have $s=0$ so all numbers are equal to $0$ and there isn't any number equal to $49$.</p><p>In the second test case, we have $s=1$. There are two possible sequences: $[0, 1]$ or $[1, 0]$. In both cases, the number $1$ appears just once. </p><p>In the third test case, we have $s=12$, which is the maximum possible value of $s$ for this case. Thus, the number $4$ appears $3$ times in the sequence.</p>
