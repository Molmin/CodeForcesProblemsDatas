## Description

<div><p>Businessman <span class="tex-font-style-it">Divan</span> loves chocolate! Today he came to a store to buy some chocolate. Like all businessmen, <span class="tex-font-style-it">Divan</span> knows the value of money, so he will not buy too expensive chocolate. At the same time, too cheap chocolate tastes bad, so he will not buy it as well.</p><p>The store he came to has $n$ different chocolate bars, and the price of the $i$-th chocolate bar is $a_i$ dollars. <span class="tex-font-style-it">Divan</span> considers a chocolate bar too expensive if it costs strictly more than $r$ dollars. Similarly, he considers a bar of chocolate to be too cheap if it costs strictly less than $l$ dollars. Divan will not buy too cheap or too expensive bars.</p><p><span class="tex-font-style-it">Divan</span> is not going to spend all his money on chocolate bars, so he will spend at most $k$ dollars on chocolates.</p><p>Please determine the maximum number of chocolate bars <span class="tex-font-style-it">Divan</span> can buy.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The description of each test case consists of two lines. The first line contains integers $n$, $l$, $r$, $k$ ($1 \le n \le 100$, $1 \le l \le r \le 10^9$, $1 \le k \le 10^9$)&nbsp;— the lowest acceptable price of a chocolate, the highest acceptable price of a chocolate and Divan's total budget, respectively.</p><p>The second line contains a sequence $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) integers&nbsp;— the prices of chocolate bars in the store.</p></div><div class="output-specification"><p>For each test case print a single integer — the maximum number of chocolate bars <span class="tex-font-style-it">Divan</span> can buy.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The description of each test case consists of two lines. The first line contains integers $n$, $l$, $r$, $k$ ($1 \le n \le 100$, $1 \le l \le r \le 10^9$, $1 \le k \le 10^9$)&nbsp;— the lowest acceptable price of a chocolate, the highest acceptable price of a chocolate and Divan's total budget, respectively.</p><p>The second line contains a sequence $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) integers&nbsp;— the prices of chocolate bars in the store.</p>

## Output

<p>For each test case print a single integer — the maximum number of chocolate bars <span class="tex-font-style-it">Divan</span> can buy.</p>





```input1
8
3 1 100 100
50 100 50
6 3 5 10
1 2 3 4 5 6
6 3 5 21
1 2 3 4 5 6
10 50 69 100
20 30 40 77 1 1 12 4 70 10000
3 50 80 30
20 60 70
10 2 7 100
2 2 2 2 2 7 7 7 7 7
4 1000000000 1000000000 1000000000
1000000000 1000000000 1000000000 1000000000
1 1 1 1
1
```




```output1
2
2
3
0
0
10
1
1
```



## Note

<p>In the first example <span class="tex-font-style-it">Divan</span> can buy chocolate bars $1$ and $3$ and spend $100$ dollars on them.</p><p>In the second example <span class="tex-font-style-it">Divan</span> can buy chocolate bars $3$ and $4$ and spend $7$ dollars on them.</p><p>In the third example <span class="tex-font-style-it">Divan</span> can buy chocolate bars $3$, $4$, and $5$ for $12$ dollars.</p><p>In the fourth example <span class="tex-font-style-it">Divan</span> cannot buy any chocolate bar because each of them is either too cheap or too expensive.</p><p>In the fifth example <span class="tex-font-style-it">Divan</span> cannot buy any chocolate bar because he considers the first bar too cheap, and has no budget for the second or third.</p><p>In the sixth example <span class="tex-font-style-it">Divan</span> can buy all the chocolate bars in the shop.</p>
