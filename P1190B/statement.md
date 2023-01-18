## Description

<div><p>Tokitsukaze and CSL are playing a little game of stones.</p><p>In the beginning, there are $n$ piles of stones, the $i$-th pile of which has $a_i$ stones. The two players take turns making moves. Tokitsukaze moves first. On each turn the player chooses a nonempty pile and removes exactly one stone from the pile. A player loses if all of the piles are empty before his turn, or if after removing the stone, two piles (possibly empty) contain the same number of stones. Supposing that both players play optimally, who will win the game?</p><p>Consider an example: $n=3$ and sizes of piles are $a_1=2$, $a_2=3$, $a_3=0$. It is impossible to choose the empty pile, so Tokitsukaze has two choices: the first and the second piles. If she chooses the first pile then the state will be $[1, 3, 0]$ and it is a good move. But if she chooses the second pile then the state will be $[2, 2, 0]$ and she immediately loses. So the only good move for her is to choose the first pile. </p><p>Supposing that both players always take their best moves and never make mistakes, who will win the game?</p><p>Note that even if there are two piles with the same number of stones at the beginning, Tokitsukaze may still be able to make a valid first move. It is only necessary that there are no two piles with the same number of stones after she moves.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of piles.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_1, a_2, \ldots, a_n \le 10^9$), which mean the $i$-th pile has $a_i$ stones.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">sjfnb</span>" (without quotes) if Tokitsukaze will win, or "<span class="tex-font-style-tt">cslnb</span>" (without quotes) if CSL will win. Note the output characters are case-sensitive.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of piles.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_1, a_2, \ldots, a_n \le 10^9$), which mean the $i$-th pile has $a_i$ stones.</p>

## Output

<p>Print "<span class="tex-font-style-tt">sjfnb</span>" (without quotes) if Tokitsukaze will win, or "<span class="tex-font-style-tt">cslnb</span>" (without quotes) if CSL will win. Note the output characters are case-sensitive.</p>





```input1
1
0
```




```input2
2
1 0
```




```input3
2
2 2
```




```input4
3
2 3 1
```




```output1
cslnb
```




```output2
cslnb
```




```output3
sjfnb
```




```output4
sjfnb
```



## Note

<p>In the first example, Tokitsukaze cannot take any stone, so CSL will win.</p><p>In the second example, Tokitsukaze can only take a stone from the first pile, and then, even though they have no stone, these two piles will have the same number of stones, which implies CSL will win.</p><p>In the third example, Tokitsukaze will win. Here is one of the optimal ways:</p><ul> <li> Firstly, Tokitsukaze can choose the first pile and take a stone from that pile. </li><li> Then, CSL can only choose the first pile, because if he chooses the second pile, he will lose immediately. </li><li> Finally, Tokitsukaze can choose the second pile, and then CSL will have no choice but to lose. </li></ul><p>In the fourth example, they only have one good choice at any time, so Tokitsukaze can make the game lasting as long as possible and finally win.</p>
