## Description

<div><p>Alice and Bob are playing a game. There are $n$ cells in a row. Initially each cell is either red or blue. Alice goes first.</p><p>On each turn, Alice chooses two neighbouring cells which contain at least one red cell, and paints that two cells white. Then, Bob chooses two neighbouring cells which contain at least one blue cell, and paints that two cells white. The player who cannot make a move loses.</p><p>Find the winner if both Alice and Bob play optimally.</p><p>Note that a chosen cell can be white, as long as the other cell satisfies the constraints.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of test cases follows.</p><p>For each test case, the first line contains an integer $n$ ($2 \leq n \leq 5 \cdot 10^5$) — the number of cells.</p><p>The second line contains a string $s$ of length $n$ — the initial state of the cells. The $i$-th cell is red if $s_i = $ <span class="tex-font-style-tt">R</span>, blue if $s_i = $ <span class="tex-font-style-tt">B</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the name of the winner on a separate line.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 10^4$) — the number of test cases. Description of test cases follows.</p><p>For each test case, the first line contains an integer $n$ ($2 \leq n \leq 5 \cdot 10^5$) — the number of cells.</p><p>The second line contains a string $s$ of length $n$ — the initial state of the cells. The $i$-th cell is red if $s_i = $ <span class="tex-font-style-tt">R</span>, blue if $s_i = $ <span class="tex-font-style-tt">B</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, output the name of the winner on a separate line.</p>





```input1|2,3,6,7,10,11,14,15
8
3
BRB
5
RRBBB
6
RBRBRB
8
BBRRBRRB
6
BRRBRB
12
RBRBRBRBRRBB
12
RBRBRBRBBBRR
4
RBBR
```




```output1
Bob
Bob
Alice
Alice
Alice
Alice
Bob
Bob
```



## Note

<p>In the notes, the cell numbers increase from left to right.</p><p>In the first testcase for Alice, she has two choices: paint the first and the second cells, or paint the second and the third cells. No matter what choice Alice makes, there will be exactly one blue cell after Alice's move. Bob just needs to paint the blue cell and its neighbour, then every cell will be white and Alice can't make a move. So Bob is the winner.</p><p>In the second testcase no matter what Alice chooses, Bob can choose to paint the fourth and fifth cells in $2$ turns.</p><p>In the third testcase at first, Alice paints the third and the fourth cells. It doesn't matter if Bob paints the first and the second cells or the fifth and sixth cells, as Alice can paint the other two cells.</p><p>In the fourth testcase at first, Alice paints the second and the third cells. If Bob paints the fifth and the sixth cells or the fourth and the fifth cells, then Alice paints the seventh and the eighth cells. If Bob paints the seventh and the eighth cells, then Alice paints the fifth and the sixth cells.</p><p>In the fifth Alice chooses the middle two cells at first, then Bob obviously has only two options, whichever variant he chooses, Alice can choose the other one and win.</p><p>In the eighth no matter what Alice chooses, Bob can choose the other two symmetrical cells.</p>
