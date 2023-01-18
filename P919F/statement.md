## Description

<div><p>Imagine that Alice is playing a card game with her friend Bob. They both have exactly $8$ cards and there is an integer on each card, ranging from $0$ to $4$. In each round, Alice or Bob in turns choose two cards from different players, let them be $a$ and $b$, where $a$ is the number on the player's card, and $b$ is the number on the opponent's card. It is necessary that $a \cdot b \ne 0$. Then they calculate $c = (a + b) \bmod 5$ and replace the number $a$ with $c$. The player who ends up with numbers on all $8$ cards being $0$, wins.</p><p>Now Alice wants to know who wins in some situations. She will give you her cards' numbers, Bob's cards' numbers and the person playing the first round. Your task is to determine who wins if both of them choose the best operation in their rounds.</p></div><div class="input-specification"><p>The first line contains one positive integer $T$ ($1 \leq T \leq 100\,000$), denoting the number of situations you need to consider.</p><p>The following lines describe those $T$ situations. For each situation:</p><ul> <li> The first line contains a non-negative integer $f$ ($0 \leq f \leq 1$), where $f = 0$ means that Alice plays first and $f = 1$ means Bob plays first. </li><li> The second line contains $8$ non-negative integers $a_1, a_2, \ldots, a_8$ ($0 \leq a_i \leq 4$), describing Alice's cards. </li><li> The third line contains $8$ non-negative integers $b_1, b_2, \ldots, b_8$ ($0 \leq b_i \leq 4$), describing Bob's cards. </li></ul><p>We guarantee that if $f=0$, we have $\sum_{i=1}^{8}a_i \ne 0$. Also when $f=1$, $\sum_{i=1}^{8}b_i \ne 0$ holds.</p></div><div class="output-specification"><p>Output $T$ lines. For each situation, determine who wins. Output </p><ul> <li> "<span class="tex-font-style-tt">Alice</span>" (without quotes) if Alice wins. </li><li> "<span class="tex-font-style-tt">Bob</span>" (without quotes) if Bob wins. </li><li> "<span class="tex-font-style-tt">Deal</span>" (without quotes) if it gets into a deal, i.e. no one wins. </li></ul></div>

## Input

<p>The first line contains one positive integer $T$ ($1 \leq T \leq 100\,000$), denoting the number of situations you need to consider.</p><p>The following lines describe those $T$ situations. For each situation:</p><ul> <li> The first line contains a non-negative integer $f$ ($0 \leq f \leq 1$), where $f = 0$ means that Alice plays first and $f = 1$ means Bob plays first. </li><li> The second line contains $8$ non-negative integers $a_1, a_2, \ldots, a_8$ ($0 \leq a_i \leq 4$), describing Alice's cards. </li><li> The third line contains $8$ non-negative integers $b_1, b_2, \ldots, b_8$ ($0 \leq b_i \leq 4$), describing Bob's cards. </li></ul><p>We guarantee that if $f=0$, we have $\sum_{i=1}^{8}a_i \ne 0$. Also when $f=1$, $\sum_{i=1}^{8}b_i \ne 0$ holds.</p>

## Output

<p>Output $T$ lines. For each situation, determine who wins. Output </p><ul> <li> "<span class="tex-font-style-tt">Alice</span>" (without quotes) if Alice wins. </li><li> "<span class="tex-font-style-tt">Bob</span>" (without quotes) if Bob wins. </li><li> "<span class="tex-font-style-tt">Deal</span>" (without quotes) if it gets into a deal, i.e. no one wins. </li></ul>





```input1
4
1
0 0 0 0 0 0 0 0
1 2 3 4 1 2 3 4
1
0 0 0 1 0 0 0 0
0 0 0 0 4 0 0 0
0
1 0 0 0 0 0 0 0
0 0 0 4 0 0 2 0
1
1 1 1 1 1 1 1 1
1 1 1 1 1 1 1 1

```




```output1
Alice
Bob
Alice
Deal

```



## Note

<p>In the first situation, Alice has all her numbers $0$. So she wins immediately.</p><p>In the second situation, Bob picks the numbers $4$ and $1$. Because we have $(4 + 1) \bmod 5 = 0$, Bob wins after this operation.</p><p>In the third situation, Alice picks the numbers $1$ and $4$. She wins after this operation.</p><p>In the fourth situation, we can prove that it falls into a loop.</p>
