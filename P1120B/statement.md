## Description

<div><p>One player came to a casino and found a slot machine where everything depends only on how he plays. The rules follow.</p><p>A positive integer $a$ is initially on the screen. The player can put a coin into the machine and then add $1$ to or subtract $1$ from any two adjacent digits. All digits must remain from $0$ to $9$ after this operation, and the leading digit must not equal zero. In other words, it is forbidden to add $1$ to $9$, to subtract $1$ from $0$ and to subtract $1$ from the leading $1$. Once the number on the screen becomes equal to $b$, the player wins the jackpot. $a$ and $b$ have the same number of digits.</p><p>Help the player to determine the minimal number of coins he needs to spend in order to win the jackpot and tell how to play.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$) standing for the length of numbers $a$ and $b$.</p><p>The next two lines contain numbers $a$ and $b$, each one on a separate line ($10^{n-1} \le a, b &lt; 10^n$).</p></div><div class="output-specification"><p>If it is impossible to win the jackpot, print a single integer $-1$.</p><p>Otherwise, the first line must contain the minimal possible number $c$ of coins the player has to spend.</p><p>$\min(c, 10^5)$ lines should follow, $i$-th of them containing two integers $d_i$ and $s_i$ ($1\le d_i\le n - 1$, $s_i = \pm 1$) denoting that on the $i$-th step the player should add $s_i$ to the $d_i$-th and $(d_i + 1)$-st digits from the left (e. g. $d_i = 1$ means that two leading digits change while $d_i = n - 1$ means that there are two trailing digits which change).</p><p>Please notice that the answer may be very big and in case $c &gt; 10^5$ you should print only the first $10^5$ moves. Your answer is considered correct if it is possible to finish your printed moves to win the jackpot in the minimal possible number of coins. In particular, if there are multiple ways to do this, you can output any of them.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$) standing for the length of numbers $a$ and $b$.</p><p>The next two lines contain numbers $a$ and $b$, each one on a separate line ($10^{n-1} \le a, b &lt; 10^n$).</p>

## Output

<p>If it is impossible to win the jackpot, print a single integer $-1$.</p><p>Otherwise, the first line must contain the minimal possible number $c$ of coins the player has to spend.</p><p>$\min(c, 10^5)$ lines should follow, $i$-th of them containing two integers $d_i$ and $s_i$ ($1\le d_i\le n - 1$, $s_i = \pm 1$) denoting that on the $i$-th step the player should add $s_i$ to the $d_i$-th and $(d_i + 1)$-st digits from the left (e. g. $d_i = 1$ means that two leading digits change while $d_i = n - 1$ means that there are two trailing digits which change).</p><p>Please notice that the answer may be very big and in case $c &gt; 10^5$ you should print only the first $10^5$ moves. Your answer is considered correct if it is possible to finish your printed moves to win the jackpot in the minimal possible number of coins. In particular, if there are multiple ways to do this, you can output any of them.</p>





```input1
3
223
322
```




```input2
2
20
42
```




```input3
2
35
44
```




```output1
2
1 1
2 -1
```




```output2
2
1 1
1 1
```




```output3
-1
```



## Note

<p>In the first example, we can make a <span class="tex-font-style-tt">+1</span> operation on the two first digits, transforming number $\textbf{22}3$ into $\textbf{33}3$, and then make a <span class="tex-font-style-tt">-1</span> operation on the last two digits, transforming $3\textbf{33}$ into $3\textbf{22}$.</p><p>It's also possible to do these operations in reverse order, which makes another correct answer.</p><p>In the last example, one can show that it's impossible to transform $35$ into $44$.</p>
