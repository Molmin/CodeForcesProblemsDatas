## Description

<div><p>A cooperative game is played by $m$ people. In the game, there are $3m$ sheets of paper: $m$ sheets with letter '<span class="tex-font-style-tt">w</span>', $m$ sheets with letter '<span class="tex-font-style-tt">i</span>', and $m$ sheets with letter '<span class="tex-font-style-tt">n</span>'.</p><p>Initially, each person is given three sheets (possibly with equal letters).</p><p>The goal of the game is to allow each of the $m$ people to spell the word "<span class="tex-font-style-tt">win</span>" using their sheets of paper. In other words, everyone should have one sheet with letter '<span class="tex-font-style-tt">w</span>', one sheet with letter '<span class="tex-font-style-tt">i</span>', and one sheet with letter '<span class="tex-font-style-tt">n</span>'.</p><p>To achieve the goal, people can make <span class="tex-font-style-it">exchanges</span>. Two people participate in each exchange. Both of them choose exactly one sheet of paper from the three sheets they own and exchange it with each other.</p><p>Find the shortest sequence of exchanges after which everyone has one '<span class="tex-font-style-tt">w</span>', one '<span class="tex-font-style-tt">i</span>', and one '<span class="tex-font-style-tt">n</span>'.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $m$&nbsp;($2 \le m \le 10^5$)&nbsp;— the number of people.</p><p>The $i$-th of the next $m$ lines contains a string $s_i$ of length $3$ consisting of lowercase English letters '<span class="tex-font-style-tt">w</span>', '<span class="tex-font-style-tt">i</span>', and '<span class="tex-font-style-tt">n</span>', denoting the letters person $i$ has on their sheets of paper at the beginning of the game, in arbitrary order.</p><p>Each of the letters '<span class="tex-font-style-tt">w</span>', '<span class="tex-font-style-tt">i</span>', and '<span class="tex-font-style-tt">n</span>' appears on the sheets of paper exactly $m$ times in total.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a non-negative integer $k$&nbsp;— the smallest number of exchanges people need to make everyone have one '<span class="tex-font-style-tt">w</span>', one '<span class="tex-font-style-tt">i</span>', and one '<span class="tex-font-style-tt">n</span>'.</p><p>In each of the next $k$ lines print four tokens $a_1$ $c_1$ $a_2$ $c_2$, describing the exchanges in chronological order ($1 \le a_1, a_2 \le m$; $a_1 \ne a_2$; $c_1, c_2$ are one of $\{\mathtt{w}, \mathtt{i}, \mathtt{n}\}$): person $a_1$ gives letter $c_1$ to person $a_2$, while person $a_2$ gives letter $c_2$ to person $a_1$ at the same time.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $m$&nbsp;($2 \le m \le 10^5$)&nbsp;— the number of people.</p><p>The $i$-th of the next $m$ lines contains a string $s_i$ of length $3$ consisting of lowercase English letters '<span class="tex-font-style-tt">w</span>', '<span class="tex-font-style-tt">i</span>', and '<span class="tex-font-style-tt">n</span>', denoting the letters person $i$ has on their sheets of paper at the beginning of the game, in arbitrary order.</p><p>Each of the letters '<span class="tex-font-style-tt">w</span>', '<span class="tex-font-style-tt">i</span>', and '<span class="tex-font-style-tt">n</span>' appears on the sheets of paper exactly $m$ times in total.</p><p>It is guaranteed that the sum of $m$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a non-negative integer $k$&nbsp;— the smallest number of exchanges people need to make everyone have one '<span class="tex-font-style-tt">w</span>', one '<span class="tex-font-style-tt">i</span>', and one '<span class="tex-font-style-tt">n</span>'.</p><p>In each of the next $k$ lines print four tokens $a_1$ $c_1$ $a_2$ $c_2$, describing the exchanges in chronological order ($1 \le a_1, a_2 \le m$; $a_1 \ne a_2$; $c_1, c_2$ are one of $\{\mathtt{w}, \mathtt{i}, \mathtt{n}\}$): person $a_1$ gives letter $c_1$ to person $a_2$, while person $a_2$ gives letter $c_2$ to person $a_1$ at the same time.</p><p>If there are multiple solutions, print any.</p>





```input1|2,3,4,9,10,11,12,13
3
2
nwi
inw
3
inn
nww
wii
4
win
www
iii
nnn
```




```output1
0
2
2 w 3 i
3 w 1 n
3
2 w 3 i
2 w 4 n
3 i 4 n
```


