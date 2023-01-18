## Description

<div><p>You are given a garland consisting of $n$ lamps. States of the lamps are represented by the string $s$ of length $n$. The $i$-th character of the string $s_i$ equals '<span class="tex-font-style-tt">0</span>' if the $i$-th lamp is turned off or '<span class="tex-font-style-tt">1</span>' if the $i$-th lamp is turned on. You are also given a positive integer $k$.</p><p>In one move, you can choose <span class="tex-font-style-bf">one lamp</span> and change its state (i.e. turn it on if it is turned off and vice versa).</p><p>The garland is called $k$-periodic if the distance between <span class="tex-font-style-bf">each pair of adjacent turned on lamps</span> is <span class="tex-font-style-bf">exactly</span> $k$. Consider the case $k=3$. Then garlands "<span class="tex-font-style-tt">00010010</span>", "<span class="tex-font-style-tt">1001001</span>", "<span class="tex-font-style-tt">00010</span>" and "<span class="tex-font-style-tt">0</span>" are good but garlands "<span class="tex-font-style-tt">00101001</span>", "<span class="tex-font-style-tt">1000001</span>" and "<span class="tex-font-style-tt">01001100</span>" are not. Note that <span class="tex-font-style-bf">the garland is not cyclic</span>, i.e. the first turned on lamp is not going after the last turned on lamp and vice versa.</p><p>Your task is to find the <span class="tex-font-style-bf">minimum</span> number of moves you need to make to obtain $k$-periodic garland from the given one.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 25~ 000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $k$ ($1 \le n \le 10^6; 1 \le k \le n$) — the length of $s$ and the required period. The second line of the test case contains the string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ ($\sum n \le 10^6$).</p></div><div class="output-specification"><p>For each test case, print the answer — the <span class="tex-font-style-bf">minimum</span> number of moves you need to make to obtain $k$-periodic garland from the given one.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 25~ 000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $k$ ($1 \le n \le 10^6; 1 \le k \le n$) — the length of $s$ and the required period. The second line of the test case contains the string $s$ consisting of $n$ characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^6$ ($\sum n \le 10^6$).</p>

## Output

<p>For each test case, print the answer — the <span class="tex-font-style-bf">minimum</span> number of moves you need to make to obtain $k$-periodic garland from the given one.</p>





```input1
6
9 2
010001010
9 3
111100000
7 4
1111111
10 3
1001110101
1 1
1
1 1
0
```




```output1
1
2
5
4
0
0
```


