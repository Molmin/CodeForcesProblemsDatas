## Description

<div><p>There are $n$ equidistant antennas on a line, numbered from $1$ to $n$. Each antenna has a power rating, the power of the $i$-th antenna is $p_i$. </p><p>The $i$-th and the $j$-th antenna can communicate directly if and only if their distance is at most the minimum of their powers, i.e., $|i-j| \leq \min(p_i, p_j)$. Sending a message directly between two such antennas takes $1$ second.</p><p>What is the minimum amount of time necessary to send a message from antenna $a$ to antenna $b$, possibly using other antennas as relays?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100\,000$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains three integers $n$, $a$, $b$ ($1 \leq a, b \leq n \leq 200\,000$) — the number of antennas, and the origin and target antenna. </p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \leq p_i \leq n$) — the powers of the antennas.</p><p>The sum of the values of $n$ over all test cases does not exceed $200\,000$. </p></div><div class="output-specification"><p>For each test case, print the number of seconds needed to trasmit a message from $a$ to $b$. It can be shown that under the problem constraints, it is always possible to send such a message.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1\le t\le 100\,000$) — the number of test cases. The descriptions of the $t$ test cases follow.</p><p>The first line of each test case contains three integers $n$, $a$, $b$ ($1 \leq a, b \leq n \leq 200\,000$) — the number of antennas, and the origin and target antenna. </p><p>The second line contains $n$ integers $p_1, p_2, \dots, p_n$ ($1 \leq p_i \leq n$) — the powers of the antennas.</p><p>The sum of the values of $n$ over all test cases does not exceed $200\,000$. </p>

## Output

<p>For each test case, print the number of seconds needed to trasmit a message from $a$ to $b$. It can be shown that under the problem constraints, it is always possible to send such a message.</p>





```input1|2,3,6,7
3
10 2 9
4 1 1 1 5 1 1 1 1 5
1 1 1
1
3 1 3
3 3 1
```




```output1
4
0
2
```



## Note

<p>In the <span class="tex-font-style-bf">first test case</span>, we must send a message from antenna $2$ to antenna $9$. A sequence of communications requiring $4$ seconds, which is the minimum possible amount of time, is the following: </p><ul> <li> In $1$ second we send the message from antenna $2$ to antenna $1$. This is possible since $|2-1|\le \min(1, 4) = \min(p_2, p_1)$. </li><li> In $1$ second we send the message from antenna $1$ to antenna $5$. This is possible since $|1-5|\le \min(4, 5) = \min(p_1, p_5)$. </li><li> In $1$ second we send the message from antenna $5$ to antenna $10$. This is possible since $|5-10|\le \min(5, 5) = \min(p_5, p_{10})$. </li><li> In $1$ second we send the message from antenna $10$ to antenna $9$. This is possible since $|10-9|\le \min(5, 1) = \min(p_{10}, p_9)$. </li></ul>
