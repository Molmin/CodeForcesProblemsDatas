## Description

<div><p>There are two currencies: pebbles and beads. Initially you have $a$ pebbles, $b$ beads.</p><p>There are $n$ days, each day you can exchange one currency for another at some exchange rate.</p><p>On day $i$, you can exchange $-p_i \leq x \leq p_i$ pebbles for $-q_i \leq y \leq q_i$ beads or vice versa. It's allowed not to perform an exchange at all. Meanwhile, if you perform an exchange, the proportion $x \cdot q_i = -y \cdot p_i$ must be fulfilled. Fractional exchanges are allowed.</p><p>You can perform no more than one such exchange in one day. The numbers of pebbles and beads you have must always remain non-negative.</p><p>Please solve the following $n$ problems independently: for each day $i$, output the maximum number of pebbles that you can have at the end of day $i$ if you perform exchanges optimally.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^3$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains three integers $n$, $a$ and $b$ ($1 \le n \le 300\,000$, $0 \le a, b \le 10^9$) — the number of days and the initial number of pebbles and beads respectively.</p><p>The second line of each test case contains $n$ integers: $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le 10^9$).</p><p>The third line of each test case contains $n$ integers: $q_1, q_2, \ldots, q_n$ ($1 \le q_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $300\,000$.</p></div><div class="output-specification"><p>Output $n$ numbers — the maximum number of pebbles at the end of each day.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{\left|a - b\right|}{\max(1, \left|b\right|)} \le 10^{-6}$.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^3$) — the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains three integers $n$, $a$ and $b$ ($1 \le n \le 300\,000$, $0 \le a, b \le 10^9$) — the number of days and the initial number of pebbles and beads respectively.</p><p>The second line of each test case contains $n$ integers: $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le 10^9$).</p><p>The third line of each test case contains $n$ integers: $q_1, q_2, \ldots, q_n$ ($1 \le q_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $300\,000$.</p>

## Output

<p>Output $n$ numbers — the maximum number of pebbles at the end of each day.</p><p>Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{\left|a - b\right|}{\max(1, \left|b\right|)} \le 10^{-6}$.</p>





```input1|2,3,4,8,9,10
3
2 6 0
2 3
4 2
3 0 6
4 2 10
2 3 10
1 10 10
33
1000
```




```output1
6
8
4
6
9.000000
10.33
```



## Note

<p>In the image below you can see the solutions for the first two test cases. In each line there is an optimal sequence of actions for each day.</p><p>In the first test case, the optimal strategy for the first day is to do no action at all, as we can only decrease the number of pebbles. The optimal strategy for the second day is at first to exchange $1$ pebble for $2$ beads, which is a correct exchange, since $1 \cdot 4 = 2 \cdot 2$, and then to exchange $2$ beads for $3$ pebbles.</p><center> <img class="tex-graphics" src="file://1BWM3qaj.png" style="max-width: 100.0%;max-height: 100.0%;" width="832px"> </center>
