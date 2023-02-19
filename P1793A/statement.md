## Description

<div><p>The famous store "Second Food" sells groceries only two days a month. And the prices in each of days differ. You wanted to buy $n$ kilos of potatoes for a month. You know that on the first day of the month $1$ kilo of potatoes costs $a$ coins, and on the second day $b$ coins. In "Second Food" you can buy any <span class="tex-font-style-bf">integer</span> kilograms of potatoes.</p><p>Fortunately, "Second Food" has announced a promotion for potatoes, which is valid only on the first day of the month — for each $m$ kilos of potatoes you buy, you get $1$ kilo as a gift! In other words, you can get $m + 1$ kilograms by paying for $m$ kilograms.</p><p>Find the minimum number of coins that you have to spend to buy <span class="tex-font-style-bf">at least</span> $n$ kilos of potatoes.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $a$ and $b$ $(1 \leq a, b \leq 10^9)$ — the prices of $1$ kilo of potatoes on the first and second days, respectively.</p><p>The second line contains two integers $n$ and $m$ $(1 \leq n, m \leq 10^9)$ — the required amount of potatoes to buy and the amount of potatoes to use the promotion.</p></div><div class="output-specification"><p>For each test case print one integer — the minimum number of coins that you have to pay to buy at least $n$ kilos of potatoes.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $a$ and $b$ $(1 \leq a, b \leq 10^9)$ — the prices of $1$ kilo of potatoes on the first and second days, respectively.</p><p>The second line contains two integers $n$ and $m$ $(1 \leq n, m \leq 10^9)$ — the required amount of potatoes to buy and the amount of potatoes to use the promotion.</p>

## Output

<p>For each test case print one integer — the minimum number of coins that you have to pay to buy at least $n$ kilos of potatoes.</p>





```input1|2,3,6,7,10,11
5
5 4
3 1
5 4
3 2
3 4
3 5
20 15
10 2
1000000000 900000000
1000000000 8
```




```output1
9
10
9
135
888888888900000000
```



## Note

<p>In the first test case, on the first day you buy $1$ kilo and get $1$ more for a promotion. On the second day, you can buy $1$ kilo of potatoes. Thus, you will spend $5+4=9$ coins in total.</p><p>In the second test case, on the first day you buy $2$ kilo and get another $1$ more for a promotion. This way you will spend $2 \cdot 5 = 10$ coins.</p>
