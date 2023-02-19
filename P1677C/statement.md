## Description

<div><p>Tokitsukaze has two colorful tapes. There are $n$ distinct colors, numbered $1$ through $n$, and each color appears exactly once on each of the two tapes. Denote the color of the $i$-th position of the first tape as $ca_i$, and the color of the $i$-th position of the second tape as $cb_i$.</p><p>Now Tokitsukaze wants to select each color an integer value from $1$ to $n$, distinct for all the colors. After that she will put down the color values in each colored position on the tapes. Denote the number of the $i$-th position of the first tape as $numa_i$, and the number of the $i$-th position of the second tape as $numb_i$.</p><center> <img class="tex-graphics" src="file://aVmRGJyO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For example, for the above picture, assuming that the color red has value $x$ ($1 \leq x \leq n$), it appears at the $1$-st position of the first tape and the $3$-rd position of the second tape, so $numa_1=numb_3=x$.</p><p>Note that each color $i$ from $1$ to $n$ should have a <span class="tex-font-style-bf">distinct</span> value, and the same color which appears in both tapes has the same value. </p><p>After labeling each color, the beauty of the two tapes is calculated as $$\sum_{i=1}^{n}|numa_i-numb_i|.$$</p><p>Please help Tokitsukaze to find the highest possible beauty. </p></div><div class="input-specification"><p>The first contains a single positive integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains a single integer $n$ ($1\leq n \leq 10^5$)&nbsp;— the number of colors.</p><p>The second line contains $n$ integers $ca_1, ca_2, \ldots, ca_n$ ($1 \leq ca_i \leq n$)&nbsp;— the color of each position of the first tape. It is guaranteed that $ca$ is a permutation.</p><p>The third line contains $n$ integers $cb_1, cb_2, \ldots, cb_n$ ($1 \leq cb_i \leq n$)&nbsp;— the color of each position of the second tape. It is guaranteed that $cb$ is a permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^{5}$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the highest possible beauty.</p></div>

## Input

<p>The first contains a single positive integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>For each test case, the first line contains a single integer $n$ ($1\leq n \leq 10^5$)&nbsp;— the number of colors.</p><p>The second line contains $n$ integers $ca_1, ca_2, \ldots, ca_n$ ($1 \leq ca_i \leq n$)&nbsp;— the color of each position of the first tape. It is guaranteed that $ca$ is a permutation.</p><p>The third line contains $n$ integers $cb_1, cb_2, \ldots, cb_n$ ($1 \leq cb_i \leq n$)&nbsp;— the color of each position of the second tape. It is guaranteed that $cb$ is a permutation.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^{5}$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the highest possible beauty.</p>





```input1
3
6
1 5 4 3 2 6
5 3 1 4 6 2
6
3 5 4 6 2 1
3 6 4 5 2 1
1
1
1
```




```output1
18
10
0
```



## Note

<p>An optimal solution for the first test case is shown in the following figure:</p><center> <img class="tex-graphics" src="file://ug4hi2gt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The beauty is $\left|4-3 \right|+\left|3-5 \right|+\left|2-4 \right|+\left|5-2 \right|+\left|1-6 \right|+\left|6-1 \right|=18$.</p><p>An optimal solution for the second test case is shown in the following figure:</p><center> <img class="tex-graphics" src="file://qXUOe4kr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The beauty is $\left|2-2 \right|+\left|1-6 \right|+\left|3-3 \right|+\left|6-1 \right|+\left|4-4 \right|+\left|5-5 \right|=10$.</p>
