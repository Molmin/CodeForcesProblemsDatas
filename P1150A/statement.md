## Description

<div><p>Welcome to Codeforces Stock Exchange! We're pretty limited now as we currently allow trading on one stock, Codeforces Ltd. We hope you'll still be able to make profit from the market!</p><p>In the morning, there are $n$ opportunities to buy shares. The $i$-th of them allows to buy as many shares as you want, each at the price of $s_i$ bourles.</p><p>In the evening, there are $m$ opportunities to sell shares. The $i$-th of them allows to sell as many shares as you want, each at the price of $b_i$ bourles. You can't sell more shares than you have.</p><p>It's morning now and you possess $r$ bourles and no shares.</p><p>What is the maximum number of bourles you can hold after the evening?</p></div><div class="input-specification"><p>The first line of the input contains three integers $n, m, r$ ($1 \leq n \leq 30$, $1 \leq m \leq 30$, $1 \leq r \leq 1000$) — the number of ways to buy the shares on the market, the number of ways to sell the shares on the market, and the number of bourles you hold now.</p><p>The next line contains $n$ integers $s_1, s_2, \dots, s_n$ ($1 \leq s_i \leq 1000$); $s_i$ indicates the opportunity to buy shares at the price of $s_i$ bourles.</p><p>The following line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \leq b_i \leq 1000$); $b_i$ indicates the opportunity to sell shares at the price of $b_i$ bourles.</p></div><div class="output-specification"><p>Output a single integer — the maximum number of bourles you can hold after the evening.</p></div>

## Input

<p>The first line of the input contains three integers $n, m, r$ ($1 \leq n \leq 30$, $1 \leq m \leq 30$, $1 \leq r \leq 1000$) — the number of ways to buy the shares on the market, the number of ways to sell the shares on the market, and the number of bourles you hold now.</p><p>The next line contains $n$ integers $s_1, s_2, \dots, s_n$ ($1 \leq s_i \leq 1000$); $s_i$ indicates the opportunity to buy shares at the price of $s_i$ bourles.</p><p>The following line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \leq b_i \leq 1000$); $b_i$ indicates the opportunity to sell shares at the price of $b_i$ bourles.</p>

## Output

<p>Output a single integer — the maximum number of bourles you can hold after the evening.</p>





```input1
3 4 11
4 2 5
4 4 5 4
```




```input2
2 2 50
5 7
4 2
```




```output1
26
```




```output2
50
```



## Note

<p>In the first example test, you have $11$ bourles in the morning. It's optimal to buy $5$ shares of a stock at the price of $2$ bourles in the morning, and then to sell all of them at the price of $5$ bourles in the evening. It's easy to verify that you'll have $26$ bourles after the evening.</p><p>In the second example test, it's optimal not to take any action.</p>
