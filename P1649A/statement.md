## Description

<div><p>You are playing a very popular computer game. The next level consists of $n$ consecutive locations, numbered from $1$ to $n$, each of them containing either land or water. It is known that the first and last locations contain land, and for completing the level you have to move from the first location to the last. Also, if you become inside a location with water, you will die, so you can only move between locations with land.</p><p>You can jump between adjacent locations for free, as well as <span class="tex-font-style-bf">no more than</span> once jump from any location with land $i$ to any location with land $i + x$, spending $x$ coins ($x \geq 0$).</p><p>Your task is to spend the minimum possible number of coins to move from the first location to the last one.</p><p>Note that this is always possible since both the first and last locations are the land locations.</p></div><div class="input-specification"><p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 100$)&nbsp;— the number of locations.</p><p>The second line of the test case contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 1$), where $a_i = 1$ means that the $i$-th location is the location with land, and $a_i = 0$ means that the $i$-th location is the location with water. It is guaranteed that $a_1 = 1$ and $a_n = 1$.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>There are several test cases in the input data. The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. This is followed by the test cases description.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 100$)&nbsp;— the number of locations.</p><p>The second line of the test case contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 1$), where $a_i = 1$ means that the $i$-th location is the location with land, and $a_i = 0$ means that the $i$-th location is the location with water. It is guaranteed that $a_1 = 1$ and $a_n = 1$.</p>

## Output

<p>For each test case print a single integer&nbsp;— the answer to the problem.</p>





```input1
3
2
1 1
5
1 0 1 0 1
4
1 0 1 1
```




```output1
0
4
2
```



## Note

<p>In the first test case, it is enough to make one free jump from the first location to the second one, which is also the last one, so the answer is $0$.</p><p>In the second test case, the only way to move from the first location to the last one is to jump between them, which will cost $4$ coins.</p><p>In the third test case, you can jump from the first location to the third for $2$ coins, and then jump to the fourth location for free, so the answer is $2$. It can be shown that this is the optimal way.</p>
