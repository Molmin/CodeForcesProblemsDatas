## Description

<div><p>You are given two integers $a$ and $b$.</p><p>In one move, you can choose some <span class="tex-font-style-bf">integer</span> $k$ from $1$ to $10$ and add it to $a$ or subtract it from $a$. In other words, you choose an integer $k \in [1; 10]$ and perform $a := a + k$ or $a := a - k$. You may use <span class="tex-font-style-bf">different</span> values of $k$ in different moves.</p><p>Your task is to find the <span class="tex-font-style-bf">minimum</span> number of moves required to obtain $b$ from $a$.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print the answer: the minimum number of moves required to obtain $b$ from $a$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2 \cdot 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>The only line of the test case contains two integers $a$ and $b$ ($1 \le a, b \le 10^9$).</p>

## Output

<p>For each test case, print the answer: the minimum number of moves required to obtain $b$ from $a$.</p>





```input1
6
5 5
13 42
18 4
1337 420
123456789 1000000000
100500 9000
```




```output1
0
3
2
92
87654322
9150
```



## Note

<p>In the first test case of the example, you don't need to do anything.</p><p>In the second test case of the example, the following sequence of moves can be applied: $13 \rightarrow 23 \rightarrow 32 \rightarrow 42$ (add $10$, add $9$, add $10$).</p><p>In the third test case of the example, the following sequence of moves can be applied: $18 \rightarrow 10 \rightarrow 4$ (subtract $8$, subtract $6$).</p>
