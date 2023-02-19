## Description

<div><p>It is given a positive integer $n$. In $1$ move, one can select any single digit and remove it (i.e. one selects some position in the number and removes the digit located at this position). The operation cannot be performed if only one digit remains. If the resulting number contains leading zeroes, they are automatically removed.</p><p>E.g. if one removes from the number $32925$ the $3$-rd digit, the resulting number will be $3225$. If one removes from the number $20099050$ the first digit, the resulting number will be $99050$ (the $2$ zeroes going next to the first digit are automatically removed).</p><p>What is the minimum number of steps to get a number such that it is divisible by $25$ and <span class="tex-font-style-bf">positive</span>? It is guaranteed that, for each $n$ occurring in the input, the answer exists. It is guaranteed that the number $n$ has no leading zeros.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing one integer $n$ ($25 \le n \le 10^{18}$). It is guaranteed that, for each $n$ occurring in the input, the answer exists. It is guaranteed that the number $n$ has no leading zeros.</p></div><div class="output-specification"><p>For each test case output on a separate line an integer $k$ ($k \ge 0$) — the minimum number of steps to get a number such that it is divisible by $25$ and positive.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing one integer $n$ ($25 \le n \le 10^{18}$). It is guaranteed that, for each $n$ occurring in the input, the answer exists. It is guaranteed that the number $n$ has no leading zeros.</p>

## Output

<p>For each test case output on a separate line an integer $k$ ($k \ge 0$) — the minimum number of steps to get a number such that it is divisible by $25$ and positive.</p>





```input1
5
100
71345
3259
50555
2050047
```




```output1
0
3
1
3
2
```



## Note

<p>In the first test case, it is already given a number divisible by $25$.</p><p>In the second test case, we can remove the digits $1$, $3$, and $4$ to get the number $75$.</p><p>In the third test case, it's enough to remove the last digit to get the number $325$.</p><p>In the fourth test case, we can remove the three last digits to get the number $50$.</p><p>In the fifth test case, it's enough to remove the digits $4$ and $7$.</p>
