## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference is the constraints on $n$, $m$ and $t$. You can make hacks only if all versions of the problem are solved.</span></p><p>Alice and Bob are given the numbers $n$, $m$ and $k$, and play a game as follows:</p><p>The game has a score that Alice tries to maximize, and Bob tries to minimize. The score is initially $0$. The game consists of $n$ turns. Each turn, Alice picks a <span class="tex-font-style-bf">real</span> number from $0$ to $k$ (inclusive) which Bob either adds to or subtracts from the score of the game. But throughout the game, Bob has to choose to add at least $m$ out of the $n$ turns.</p><p>Bob gets to know which number Alice picked before deciding whether to add or subtract the number from the score, and Alice gets to know whether Bob added or subtracted the number for the previous turn before picking the number for the current turn (except on the first turn since there was no previous turn).</p><p>If Alice and Bob play optimally, what will the final score of the game be?</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. The description of test cases follows.</p><p>Each test case consists of a single line containing the three integers, $n$, $m$, and $k$ ($1 \le m \le n \le 10^6, 0 \le k &lt; 10^9 + 7$) — the number of turns, how many of those turns Bob <span class="tex-font-style-it">has to</span> add, and the biggest number Alice can choose, respectively.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case output a single <span class="tex-font-style-bf">integer</span> number — the score of the optimal game modulo $10^9 + 7$.</p><p>Formally, let $M = 10^9 + 7$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. The description of test cases follows.</p><p>Each test case consists of a single line containing the three integers, $n$, $m$, and $k$ ($1 \le m \le n \le 10^6, 0 \le k &lt; 10^9 + 7$) — the number of turns, how many of those turns Bob <span class="tex-font-style-it">has to</span> add, and the biggest number Alice can choose, respectively.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case output a single <span class="tex-font-style-bf">integer</span> number — the score of the optimal game modulo $10^9 + 7$.</p><p>Formally, let $M = 10^9 + 7$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p>





```input1
7
3 3 2
2 1 10
6 3 10
6 4 10
100 1 1
4 4 0
69 4 20
```




```output1
6
5
375000012
500000026
958557139
0
49735962
```



## Note

<p>In the first test case, the entire game has $3$ turns, and since $m = 3$, Bob has to add in each of them. Therefore Alice should pick the biggest number she can, which is $k = 2$, every turn.</p><p>In the third test case, Alice has a strategy to guarantee a score of $\frac{75}{8} \equiv 375000012 \pmod{10^9 + 7}$.</p><p>In the fourth test case, Alice has a strategy to guarantee a score of $\frac{45}{2} \equiv 500000026 \pmod{10^9 + 7}$.</p>
