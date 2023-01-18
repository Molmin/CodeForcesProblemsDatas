## Description

<div><p>You are playing a computer card game called Splay the Sire. Currently you are struggling to defeat the final boss of the game.</p><p>The boss battle consists of $n$ turns. During each turn, you will get several cards. Each card has two parameters: its cost $c_i$ and damage $d_i$. You may play some of your cards during each turn in some sequence (you choose the cards and the exact order they are played), as long as <span class="tex-font-style-bf">the total cost of the cards you play during the turn does not exceed $3$</span>. After playing some (possibly zero) cards, you end your turn, and <span class="tex-font-style-bf">all cards you didn't play are discarded</span>. Note that you can use each card <span class="tex-font-style-bf">at most once</span>.</p><p>Your character has also found an artifact that boosts the damage of some of your actions: every $10$-th card you play deals double damage.</p><p>What is the maximum possible damage you can deal during $n$ turns?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of turns.</p><p>Then $n$ blocks of input follow, the $i$-th block representing the cards you get during the $i$-th turn.</p><p>Each block begins with a line containing one integer $k_i$ ($1 \le k_i \le 2 \cdot 10^5$) — the number of cards you get during $i$-th turn. Then $k_i$ lines follow, each containing two integers $c_j$ and $d_j$ ($1 \le c_j \le 3$, $1 \le d_j \le 10^9$) — the parameters of the corresponding card.</p><p>It is guaranteed that $\sum \limits_{i = 1}^{n} k_i \le 2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print one integer — the maximum damage you may deal.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of turns.</p><p>Then $n$ blocks of input follow, the $i$-th block representing the cards you get during the $i$-th turn.</p><p>Each block begins with a line containing one integer $k_i$ ($1 \le k_i \le 2 \cdot 10^5$) — the number of cards you get during $i$-th turn. Then $k_i$ lines follow, each containing two integers $c_j$ and $d_j$ ($1 \le c_j \le 3$, $1 \le d_j \le 10^9$) — the parameters of the corresponding card.</p><p>It is guaranteed that $\sum \limits_{i = 1}^{n} k_i \le 2 \cdot 10^5$.</p>

## Output

<p>Print one integer — the maximum damage you may deal.</p>





```input1
5
3
1 6
1 7
1 5
2
1 4
1 3
3
1 10
3 5
2 3
3
1 15
2 4
1 10
1
1 100
```




```output1
263
```



## Note

<p>In the example test the best course of action is as follows:</p><p>During the first turn, play all three cards in any order and deal $18$ damage.</p><p>During the second turn, play both cards and deal $7$ damage.</p><p>During the third turn, play the first and the third card and deal $13$ damage.</p><p>During the fourth turn, play the first and the third card and deal $25$ damage.</p><p>During the fifth turn, play the only card, which will deal double damage ($200$).</p>
