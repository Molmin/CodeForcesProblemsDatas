## Description

<div><p>Dasha has $10^{100}$ coins. Recently, she found a binary string $s$ of length $n$ and some operations that allows to change this string (she can do each operation any number of times):</p><ol> <li> Replace substring <span class="tex-font-style-tt">00</span> of $s$ by <span class="tex-font-style-tt">0</span> and receive $a$ coins. </li><li> Replace substring <span class="tex-font-style-tt">11</span> of $s$ by <span class="tex-font-style-tt">1</span> and receive $b$ coins. </li><li> Remove <span class="tex-font-style-tt">0</span> from any position in $s$ and <span class="tex-font-style-bf">pay</span> $c$ coins. </li></ol><p>It turned out that while doing this operations Dasha should follow the rule:</p><ul> <li> It is forbidden to do two operations with the same parity in a row. Operations are numbered by integers $1$-$3$ in the order they are given above. </li></ul><p>Please, calculate what is the maximum profit Dasha can get by doing these operations and following this rule.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains four integers $n$, $a$, $b$, $c$ ($1 \leq n \leq 10^5, 1 \leq a, b, c \leq 10^9$).</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the total sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print the answer.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains four integers $n$, $a$, $b$, $c$ ($1 \leq n \leq 10^5, 1 \leq a, b, c \leq 10^9$).</p><p>The second line of each test case contains a binary string $s$ of length $n$.</p><p>It is guaranteed that the total sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print the answer.</p>





```input1|2,3,6,7
3
5 2 2 1
01101
6 4 3 5
110001
6 3 2 1
011110
```




```output1
3
11
4
```



## Note

<p>In the first test case one of the optimal sequences of operations is <span class="tex-font-style-tt">0<span class="tex-font-style-bf">11</span>01</span> $\rightarrow$ <span class="tex-font-style-tt">01<span class="tex-font-style-bf">0</span>1</span> $\rightarrow$ <span class="tex-font-style-tt">0<span class="tex-font-style-bf">11</span></span> $\rightarrow$ <span class="tex-font-style-tt">01</span>. This sequence of operations consists of operations $2$, $3$ and $2$ in this order. It satisfies all rules and gives profit $3$. It can be shown that it is impossible to achieve higher profit in this test case, so the answer is $3$.</p><p>In the second test case one of the optimal sequences of operations is <span class="tex-font-style-tt">110<span class="tex-font-style-bf">00</span>1</span> $\rightarrow$ <span class="tex-font-style-tt"><span class="tex-font-style-bf">11</span>001</span> $\rightarrow$ <span class="tex-font-style-tt">1<span class="tex-font-style-bf">00</span>1</span> $\rightarrow$ <span class="tex-font-style-tt">101</span>.</p><p>In the third test case one of the optimal sequences of operations is <span class="tex-font-style-tt">01<span class="tex-font-style-bf">11</span>10</span> $\rightarrow$ <span class="tex-font-style-tt"><span class="tex-font-style-bf">0</span>1110</span> $\rightarrow$ <span class="tex-font-style-tt"><span class="tex-font-style-bf">11</span>10</span> $\rightarrow$ <span class="tex-font-style-tt">11<span class="tex-font-style-bf">0</span></span> $\rightarrow$ <span class="tex-font-style-tt"><span class="tex-font-style-bf">11</span></span> $\rightarrow$ <span class="tex-font-style-tt">1</span>.</p>
