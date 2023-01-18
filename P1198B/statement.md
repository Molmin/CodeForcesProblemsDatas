## Description

<div><p>There is a country with $n$ citizens. The $i$-th of them initially has $a_{i}$ money. The government strictly controls the wealth of its citizens. Whenever a citizen makes a purchase or earns some money, they must send a receipt to the social services mentioning the amount of money they currently have.</p><p>Sometimes the government makes payouts to the poor: all citizens who have strictly less money than $x$ are paid accordingly so that after the payout they have exactly $x$ money. In this case the citizens don't send a receipt.</p><p>You know the initial wealth of every citizen and the log of all events: receipts and payouts. Restore the amount of money each citizen has after all events.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^{5}$)&nbsp;— the numer of citizens.</p><p>The next line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_{i} \le 10^{9}$)&nbsp;— the initial balances of citizens.</p><p>The next line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^{5}$)&nbsp;— the number of events.</p><p>Each of the next $q$ lines contains a single event. The events are given in chronological order.</p><p>Each event is described as either <span class="tex-font-style-tt">1 p x</span> ($1 \le p \le n$, $0 \le x \le 10^{9}$), or <span class="tex-font-style-tt">2 x</span> ($0 \le x \le 10^{9}$). In the first case we have a receipt that the balance of the $p$-th person becomes equal to $x$. In the second case we have a payoff with parameter $x$.</p></div><div class="output-specification"><p>Print $n$ integers&nbsp;— the balances of all citizens after all events.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^{5}$)&nbsp;— the numer of citizens.</p><p>The next line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($0 \le a_{i} \le 10^{9}$)&nbsp;— the initial balances of citizens.</p><p>The next line contains a single integer $q$ ($1 \le q \le 2 \cdot 10^{5}$)&nbsp;— the number of events.</p><p>Each of the next $q$ lines contains a single event. The events are given in chronological order.</p><p>Each event is described as either <span class="tex-font-style-tt">1 p x</span> ($1 \le p \le n$, $0 \le x \le 10^{9}$), or <span class="tex-font-style-tt">2 x</span> ($0 \le x \le 10^{9}$). In the first case we have a receipt that the balance of the $p$-th person becomes equal to $x$. In the second case we have a payoff with parameter $x$.</p>

## Output

<p>Print $n$ integers&nbsp;— the balances of all citizens after all events.</p>





```input1
4
1 2 3 4
3
2 3
1 2 2
2 1
```




```input2
5
3 50 2 1 10
3
1 2 0
2 8
1 3 20
```




```output1
3 2 3 4
```




```output2
8 8 20 8 10
```



## Note

<p>In the first example the balances change as follows: <span class="tex-font-style-tt">1 2 3 4</span> $\rightarrow$ <span class="tex-font-style-tt">3 3 3 4</span> $\rightarrow$ <span class="tex-font-style-tt">3 2 3 4</span> $\rightarrow$ <span class="tex-font-style-tt">3 2 3 4</span></p><p>In the second example the balances change as follows: <span class="tex-font-style-tt">3 50 2 1 10</span> $\rightarrow$ <span class="tex-font-style-tt">3 0 2 1 10</span> $\rightarrow$ <span class="tex-font-style-tt">8 8 8 8 10</span> $\rightarrow$ <span class="tex-font-style-tt">8 8 20 8 10</span></p>
