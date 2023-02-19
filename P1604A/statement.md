## Description

<div><p>Shohag has an integer sequence $a_1, a_2, \ldots, a_n$. He can perform the following operation any number of times (possibly, zero):</p><ul> <li> Select any positive integer $k$ (it can be different in different operations). </li><li> Choose any position in the sequence (possibly the beginning or end of the sequence, or in between any two elements) and insert $k$ into the sequence at this position. </li><li> This way, the sequence $a$ changes, and the next operation is performed on this changed sequence. </li></ul><p>For example, if $a=[3,3,4]$ and he selects $k = 2$, then after the operation he can obtain one of the sequences $[\underline{2},3,3,4]$, $[3,\underline{2},3,4]$, $[3,3,\underline{2},4]$, or $[3,3,4,\underline{2}]$.</p><p>Shohag wants this sequence to satisfy the following condition: for each $1 \le i \le |a|$, $a_i \le i$. Here, $|a|$ denotes the size of $a$.</p><p>Help him to find the minimum number of operations that he has to perform to achieve this goal. We can show that under the constraints of the problem it's always possible to achieve this goal in a finite number of operations.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 200$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) — the initial length of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) — the elements of the sequence.</p></div><div class="output-specification"><p>For each test case, print a single integer &nbsp;— the minimum number of operations needed to perform to achieve the goal mentioned in the statement.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 200$) &nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$) — the initial length of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) — the elements of the sequence.</p>

## Output

<p>For each test case, print a single integer &nbsp;— the minimum number of operations needed to perform to achieve the goal mentioned in the statement.</p>





```input1
4
3
1 3 4
5
1 2 5 7 4
1
1
3
69 6969 696969
```




```output1
1
3
0
696966
```



## Note

<p>In the first test case, we have to perform at least one operation, as $a_2=3&gt;2$. We can perform the operation $[1, 3, 4] \rightarrow [1, \underline{2}, 3, 4]$ (the newly inserted element is underlined), now the condition is satisfied.</p><p>In the second test case, Shohag can perform the following operations:</p><p>$[1, 2, 5, 7, 4] \rightarrow [1, 2, \underline{3}, 5, 7, 4] \rightarrow [1, 2, 3, \underline{4}, 5, 7, 4] \rightarrow [1, 2, 3, 4, 5, \underline{3}, 7, 4]$.</p><p>In the third test case, the sequence already satisfies the condition.</p>
