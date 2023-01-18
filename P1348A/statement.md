## Description

<div><p>Phoenix has $n$ coins with weights $2^1, 2^2, \dots, 2^n$. He knows that $n$ is even.</p><p>He wants to split the coins into two piles such that each pile has exactly $\frac{n}{2}$ coins and the difference of weights between the two piles is <span class="tex-font-style-bf">minimized</span>. Formally, let $a$ denote the sum of weights in the first pile, and $b$ denote the sum of weights in the second pile. Help Phoenix minimize $|a-b|$, the absolute value of $a-b$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 30$; $n$ is even)&nbsp;— the number of coins that Phoenix has. </p></div><div class="output-specification"><p>For each test case, output one integer&nbsp;— the minimum possible difference of weights between the two piles.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 30$; $n$ is even)&nbsp;— the number of coins that Phoenix has. </p>

## Output

<p>For each test case, output one integer&nbsp;— the minimum possible difference of weights between the two piles.</p>





```input1
2
2
4
```




```output1
2
6
```



## Note

<p>In the first test case, Phoenix has two coins with weights $2$ and $4$. No matter how he divides the coins, the difference will be $4-2=2$.</p><p>In the second test case, Phoenix has four coins of weight $2$, $4$, $8$, and $16$. It is optimal for Phoenix to place coins with weights $2$ and $16$ in one pile, and coins with weights $4$ and $8$ in another pile. The difference is $(2+16)-(4+8)=6$.</p>
