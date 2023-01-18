## Description

<div><p>Alice and Bob are playing a game with $n$ piles of stones. It is guaranteed that $n$ is an even number. The $i$-th pile has $a_i$ stones.</p><p>Alice and Bob will play a game alternating turns with Alice going first.</p><p>On a player's turn, they must choose <span class="tex-font-style-bf">exactly</span> $\frac{n}{2}$ nonempty piles and independently remove a positive number of stones from each of the chosen piles. They <span class="tex-font-style-bf">can</span> remove a <span class="tex-font-style-bf">different</span> number of stones from the piles in a single turn. The first player unable to make a move loses (when there are less than $\frac{n}{2}$ nonempty piles).</p><p>Given the starting configuration, determine who will win the game.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \leq n \leq 50$)&nbsp;— the number of piles. It is guaranteed that $n$ is an even number.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 50$)&nbsp;— the number of stones in the piles.</p></div><div class="output-specification"><p>Print a single string "<span class="tex-font-style-tt">Alice</span>" if Alice wins; otherwise, print "<span class="tex-font-style-tt">Bob</span>" (without double quotes).</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \leq n \leq 50$)&nbsp;— the number of piles. It is guaranteed that $n$ is an even number.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 50$)&nbsp;— the number of stones in the piles.</p>

## Output

<p>Print a single string "<span class="tex-font-style-tt">Alice</span>" if Alice wins; otherwise, print "<span class="tex-font-style-tt">Bob</span>" (without double quotes).</p>





```input1
2
8 8
```




```input2
4
3 1 4 1
```




```output1
Bob
```




```output2
Alice
```



## Note

<p>In the first example, each player can only remove stones from one pile ($\frac{2}{2}=1$). Alice loses, since Bob can copy whatever Alice does on the other pile, so Alice will run out of moves first.</p><p>In the second example, Alice can remove $2$ stones from the first pile and $3$ stones from the third pile on her first move to guarantee a win.</p>
