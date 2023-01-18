## Description

<div><p>Alice and Bob are playing yet another card game. This time the rules are the following. There are $n$ cards lying in a row in front of them. The $i$-th card has value $a_i$. </p><p>First, Alice chooses a non-empty consecutive segment of cards $[l; r]$ ($l \le r$). After that Bob removes a single card $j$ from that segment $(l \le j \le r)$. The score of the game is the total value of the remaining cards on the segment $(a_l + a_{l + 1} + \dots + a_{j - 1} + a_{j + 1} + \dots + a_{r - 1} + a_r)$. In particular, if Alice chooses a segment with just one element, then the score after Bob removes the only card is $0$.</p><p>Alice wants to make the score as big as possible. Bob takes such a card that the score is as small as possible.</p><p>What segment should Alice choose so that the score is maximum possible? Output the maximum score.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$) — the number of cards.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-30 \le a_i \le 30$) — the values on the cards.</p></div><div class="output-specification"><p>Print a single integer — the final score of the game.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$) — the number of cards.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-30 \le a_i \le 30$) — the values on the cards.</p>

## Output

<p>Print a single integer — the final score of the game.</p>





```input1
5
5 -2 10 -1 4
```




```input2
8
5 2 5 3 -30 -30 6 9
```




```input3
3
-10 6 -15
```




```output1
6
```




```output2
10
```




```output3
0
```



## Note

<p>In the first example Alice chooses a segment $[1;5]$ — the entire row of cards. Bob removes card $3$ with the value $10$ from the segment. Thus, the final score is $5 + (-2) + (-1) + 4 = 6$.</p><p>In the second example Alice chooses a segment $[1;4]$, so that Bob removes either card $1$ or $3$ with the value $5$, making the answer $5 + 2 + 3 = 10$.</p><p>In the third example Alice can choose any of the segments of length $1$: $[1;1]$, $[2;2]$ or $[3;3]$. Bob removes the only card, so the score is $0$. If Alice chooses some other segment then the answer will be less than $0$.</p>
