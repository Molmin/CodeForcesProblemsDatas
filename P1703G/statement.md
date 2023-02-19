## Description

<div><p>There are $n$ chests. The $i$-th chest contains $a_i$ coins. You need to open all $n$ chests <span class="tex-font-style-bf">in order from chest </span>$1$<span class="tex-font-style-bf"> to chest </span>$n$.</p><p>There are two types of keys you can use to open a chest: </p><ul> <li> a good key, which costs $k$ coins to use; </li><li> a bad key, which does not cost any coins, but will halve all the coins in each unopened chest, <span class="tex-font-style-bf">including the chest it is about to open</span>. The halving operation <span class="tex-font-style-bf">will round down</span> to the nearest integer for each chest halved. In other words using a bad key to open chest $i$ will do $a_i = \lfloor{\frac{a_i}{2}\rfloor}$, $a_{i+1} = \lfloor\frac{a_{i+1}}{2}\rfloor, \dots, a_n = \lfloor \frac{a_n}{2}\rfloor$; </li><li> any key (both good and bad) breaks after a usage, that is, it is a one-time use. </li></ul><p>You need to use in total $n$ keys, one for each chest. Initially, you have no coins and no keys. If you want to use a good key, then you need to buy it.</p><p>During the process, you are allowed to go into debt; for example, if you have $1$ coin, you are allowed to buy a good key worth $k=3$ coins, and your balance will become $-2$ coins.</p><p>Find the maximum number of coins you can have after opening all $n$ chests in order from chest $1$ to chest $n$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 10^5$; $0 \leq k \leq 10^9$)&nbsp;— the number of chests and the cost of a good key respectively.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 10^9$) &nbsp;— the amount of coins in each chest.</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer &nbsp;— the maximum number of coins you can obtain after opening the chests in order from chest $1$ to chest $n$.</p><p>Please note, that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \leq n \leq 10^5$; $0 \leq k \leq 10^9$)&nbsp;— the number of chests and the cost of a good key respectively.</p><p>The second line of each test case contains $n$ integers $a_i$ ($0 \leq a_i \leq 10^9$) &nbsp;— the amount of coins in each chest.</p><p>The sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output a single integer &nbsp;— the maximum number of coins you can obtain after opening the chests in order from chest $1$ to chest $n$.</p><p>Please note, that the answer for some test cases won't fit into 32-bit integer type, so you should use at least 64-bit integer type in your programming language (like <span class="tex-font-style-tt">long long</span> for C++).</p>





```input1|2,3,6,7,10,11
5
4 5
10 10 3 1
1 2
1
3 12
10 10 29
12 51
5 74 89 45 18 69 67 67 11 96 23 59
2 57
85 60
```




```output1
11
0
13
60
58
```



## Note

<p>In the first test case, one possible strategy is as follows: </p><ul> <li> Buy a good key for $5$ coins, and open chest $1$, receiving $10$ coins. Your current balance is $0 + 10 - 5 = 5$ coins. </li><li> Buy a good key for $5$ coins, and open chest $2$, receiving $10$ coins. Your current balance is $5 + 10 - 5 = 10$ coins. </li><li> Use a bad key and open chest $3$. As a result of using a bad key, the number of coins in chest $3$ becomes $\left\lfloor \frac{3}{2} \right\rfloor = 1$, and the number of coins in chest $4$ becomes $\left\lfloor \frac{1}{2} \right\rfloor = 0$. Your current balance is $10 + 1 = 11$. </li><li> Use a bad key and open chest $4$. As a result of using a bad key, the number of coins in chest $4$ becomes $\left\lfloor \frac{0}{2} \right\rfloor = 0$. Your current balance is $11 + 0 = 11$. </li></ul> At the end of the process, you have $11$ coins, which can be proven to be maximal.
