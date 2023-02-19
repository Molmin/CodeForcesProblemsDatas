## Description

<div><p>Timur has a stairway with $n$ steps. The $i$-th step is $a_i$ meters higher than its predecessor. The first step is $a_1$ meters higher than the ground, and the ground starts at $0$ meters. </p><center> <img class="tex-graphics" src="file://aNg7H5MP.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The stairs for the first test case.</span> </center><p>Timur has $q$ questions, each denoted by an integer $k_1, \dots, k_q$. For each question $k_i$, you have to print the maximum possible height Timur can achieve by climbing the steps if his legs are of length $k_i$. Timur can only climb the $j$-th step if his legs are of length at least $a_j$. In other words, $k_i \geq a_j$ for each step $j$ climbed.</p><p>Note that you should answer each question independently.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n, q$ ($1 \leq n, q \leq 2\cdot10^5$)&nbsp;— the number of steps and the number of questions, respectively.</p><p>The second line of each test case contains $n$ integers ($1 \leq a_i \leq 10^9$)&nbsp;— the height of the steps.</p><p>The third line of each test case contains $q$ integers ($0 \leq k_i \leq 10^9$)&nbsp;— the numbers for each question.</p><p>It is guaranteed that the sum of $n$ does not exceed $2\cdot10^5$, and the sum of $q$ does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output a single line containing $q$ integers, the answer for each question.</p><p>Please note, that the answer for some questions won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n, q$ ($1 \leq n, q \leq 2\cdot10^5$)&nbsp;— the number of steps and the number of questions, respectively.</p><p>The second line of each test case contains $n$ integers ($1 \leq a_i \leq 10^9$)&nbsp;— the height of the steps.</p><p>The third line of each test case contains $q$ integers ($0 \leq k_i \leq 10^9$)&nbsp;— the numbers for each question.</p><p>It is guaranteed that the sum of $n$ does not exceed $2\cdot10^5$, and the sum of $q$ does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output a single line containing $q$ integers, the answer for each question.</p><p>Please note, that the answer for some questions won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p>





```input1|2,3,4,8,9,10
3
4 5
1 2 1 5
1 2 4 9 10
2 2
1 1
0 1
3 1
1000000000 1000000000 1000000000
1000000000
```




```output1
1 4 4 9 9 
0 2 
3000000000
```



## Note

<p>Consider the first test case, pictured in the statement. </p><ul> <li> If Timur's legs have length $1$, then he can only climb stair $1$, so the highest he can reach is $1$ meter. </li><li> If Timur's legs have length $2$ or $4$, then he can only climb stairs $1$, $2$, and $3$, so the highest he can reach is $1+2+1=4$ meters. </li><li> If Timur's legs have length $9$ or $10$, then he can climb the whole staircase, so the highest he can reach is $1+2+1+5=9$ meters. </li></ul> In the first question of the second test case, Timur has no legs, so he cannot go up even a single step. <span class="tex-font-style-tt">:(</span>
