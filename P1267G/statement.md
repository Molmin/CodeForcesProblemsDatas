## Description

<div><p>Esports is a form of competitive sports using video games. Dota&nbsp;2 is one of the most popular competitive video games in Esports. Recently, a new video game Dota&nbsp;3 was released. In Dota&nbsp;3 a player can buy some relics for their hero. Relics are counters that track hero's actions and statistics in a game.</p><p>Gloria likes to play Dota&nbsp;3, so she wants to buy all $n$ available relics for her favorite hero.</p><p>Relics can be bought using an in-game currency called shards. Each relic has its own price&nbsp;— $c_i$ shards for the $i$-th relic. A player can buy a relic using one of the following options: </p><ul> <li> Pay $c_i$ shards to buy the $i$-th relic; </li><li> Pay $x$ shards and randomly get one of all $n$ relics. The probability of getting a relic is the same for all $n$ relics. If a duplicate relic is received, then the relic is recycled and $\frac{x}{2}$ shards are given back to the player. </li></ul><p>Gloria wants to buy all $n$ relics. Help her minimize the expected number of shards she spends to buy all the relics.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $x$ ($1 \le n \le 100$; $1 \le x \le 10\,000$)&nbsp;— the number of relics and the cost to receive a random relic.</p><p>The second line consists of $n$ integers $c_1, c_2, \ldots, c_n$ ($x \le c_i \le 10\,000$; $\sum{c_i} \le 10\,000$)&nbsp;— the prices of $n$&nbsp;relics.</p></div><div class="output-specification"><p>Print a single real number&nbsp;— the minimum expected number of shards that Gloria must spend to buy all the relics.</p><p>The absolute or relative error should not exceed $10^{-9}$.</p></div>

## Input

<p>The first line contains two integers $n$ and $x$ ($1 \le n \le 100$; $1 \le x \le 10\,000$)&nbsp;— the number of relics and the cost to receive a random relic.</p><p>The second line consists of $n$ integers $c_1, c_2, \ldots, c_n$ ($x \le c_i \le 10\,000$; $\sum{c_i} \le 10\,000$)&nbsp;— the prices of $n$&nbsp;relics.</p>

## Output

<p>Print a single real number&nbsp;— the minimum expected number of shards that Gloria must spend to buy all the relics.</p><p>The absolute or relative error should not exceed $10^{-9}$.</p>





```input1
2 20
25 100
```




```input2
4 30
60 50 60 80
```




```output1
47.50000000000000000
```




```output2
171.25000000000000000
```



## Note

<p>In the first example, the optimal strategy is to randomly get one of the two relics paying $20$ shards. Then there are two scenarios. </p><p>The first one happens if Gloria receives the first relic. Then she keeps getting random relics until she obtains the second relic. The expected number of shards to spend in this scenario is $20 + 30 = 50$.</p><p>In the second scenario, Gloria initially gets the second relic. Then it is better to buy the first relic for $25$ shards, so the expected number of shards to spend in this scenario is $20 + 25 = 45$.</p><p>Thus, the expected number of shards to spend is $\frac{50 + 45}{2} = 47.5$.</p>
