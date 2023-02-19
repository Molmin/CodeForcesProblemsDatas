## Description

<div><p>There are $n$ participants in a competition, participant $i$ having a strength of $s_i$. </p><p>Every participant wonders how much of an advantage they have over the other best participant. In other words, each participant $i$ wants to know the difference between $s_i$ and $s_j$, where $j$ is the strongest participant in the competition, not counting $i$ (a difference can be negative).</p><p>So, they ask you for your help! For each $i$ ($1 \leq i \leq n$) output the difference between $s_i$ and the maximum strength of any participant other than participant $i$.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated positive integers $s_1$, $s_2$, ..., $s_n$ ($1 \leq s_i \leq 10^9$)&nbsp;— the strengths of the participants.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output $n$ space-separated integers. For each $i$ ($1 \leq i \leq n$) output the difference between $s_i$ and the maximum strength of any other participant.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains an integer $n$ ($2 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The following line contains $n$ space-separated positive integers $s_1$, $s_2$, ..., $s_n$ ($1 \leq s_i \leq 10^9$)&nbsp;— the strengths of the participants.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output $n$ space-separated integers. For each $i$ ($1 \leq i \leq n$) output the difference between $s_i$ and the maximum strength of any other participant.</p>





```input1|2,3,6,7,10,11
5
4
4 7 3 5
2
1 2
5
1 2 3 4 5
3
4 9 4
4
4 4 4 4
```




```output1
-3 2 -4 -2 
-1 1 
-4 -3 -2 -1 1 
-5 5 -5 
0 0 0 0
```



## Note

<p>For the first test case:</p><ul><li> The first participant has a strength of $4$ and the largest strength of a participant different from the first one is $7$, so the answer for the first participant is $4 - 7 = -3$. </li><li> The second participant has a strength of $7$ and the largest strength of a participant different from the second one is $5$, so the answer for the second participant is $7 - 5 = 2$.</li><li> The third participant has a strength of $3$ and the largest strength of a participant different from the third one is $7$, so the answer for the third participant is $3 - 7 = -4$.</li><li> The fourth participant has a strength of $5$ and the largest strength of a participant different from the fourth one is $7$, so the answer for the fourth participant is $5 - 7 = -2$. </li></ul>
