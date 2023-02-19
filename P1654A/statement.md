## Description

<div><p>There are $n$ pieces of cake on a line. The $i$-th piece of cake has weight $a_i$ ($1 \leq i \leq n$).</p><p>The tastiness of the cake is the maximum total weight of two adjacent pieces of cake (i.&nbsp;e., $\max(a_1+a_2,\, a_2+a_3,\, \ldots,\, a_{n-1} + a_{n})$).</p><p>You want to maximize the tastiness of the cake. You are allowed to do the following operation at most once (doing more operations would ruin the cake): </p><ul> <li> Choose a contiguous subsegment $a[l, r]$ of pieces of cake ($1 \leq l \leq r \leq n$), and reverse it. </li></ul><p>The subsegment $a[l, r]$ of the array $a$ is the sequence $a_l, a_{l+1}, \dots, a_r$.</p><p>If you reverse it, the array will become $a_1, a_2, \dots, a_{l-2}, a_{l-1}, \underline{a_r}, \underline{a_{r-1}}, \underline{\dots}, \underline{a_{l+1}}, \underline{a_l}, a_{r+1}, a_{r+2}, \dots, a_{n-1}, a_n$.</p><p>For example, if the weights are initially $[5, 2, 1, 4, 7, 3]$, you can reverse the subsegment $a[2, 5]$, getting $[5, \underline{7}, \underline{4}, \underline{1}, \underline{2}, 3]$. The tastiness of the cake is now $5 + 7 = 12$ (while before the operation the tastiness was $4+7=11$).</p><p>Find the maximum tastiness of the cake after doing the operation at most once.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 50$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 1000$) — the number of pieces of cake.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — $a_i$ is the weight of the $i$-th piece of cake.</p></div><div class="output-specification"><p>For each test case, print a single integer: the maximum tastiness of the cake after doing the operation at most once.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 50$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($2 \le n \le 1000$) — the number of pieces of cake.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) — $a_i$ is the weight of the $i$-th piece of cake.</p>

## Output

<p>For each test case, print a single integer: the maximum tastiness of the cake after doing the operation at most once.</p>





```input1|2,3,6,7,10,11
5
6
5 2 1 4 7 3
3
32 78 78
3
69 54 91
8
999021 999021 999021 999021 999652 999021 999021 999021
2
1000000000 1000000000
```




```output1
12
156
160
1998673
2000000000
```



## Note

<p>In the first test case, after reversing the subsegment $a[2, 5]$, you get a cake with weights $[5, \underline{7}, \underline{4}, \underline{1}, \underline{2}, 3]$. The tastiness of the cake is now $\max(5+7, 7+4, 4+1, 1+2, 2+3) = 12$. This is the maximum possible tastiness of the cake one can obtain by performing the operation at most once.</p><p>In the second test case, it's optimal not to do any operation. The tastiness is $78+78 = 156$.</p><p>In the third test case, after reversing the subsegment $a[1, 2]$, you get a cake with weights $[\underline{54}, \underline{69}, 91]$. The tastiness of the cake is now $\max(54+69, 69+91) = 160$. There is no way to make the tastiness of the cake greater than $160$ by performing at most one operation.</p>
