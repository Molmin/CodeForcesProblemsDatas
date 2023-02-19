## Description

<div><p>Luntik has decided to try singing. He has $a$ one-minute songs, $b$ two-minute songs and $c$ three-minute songs. He wants to distribute all songs into two concerts such that every song should be included to exactly one concert.</p><p>He wants to make the absolute difference of durations of the concerts as small as possible. The duration of the concert is the sum of durations of all songs in that concert.</p><p>Please help Luntik and find the minimal possible difference in minutes between the concerts durations.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing three integers $a, b, c$ $(1 \le a, b, c \le 10^9)$&nbsp;— the number of one-minute, two-minute and three-minute songs.</p></div><div class="output-specification"><p>For each test case print the minimal possible difference in minutes between the concerts durations.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing three integers $a, b, c$ $(1 \le a, b, c \le 10^9)$&nbsp;— the number of one-minute, two-minute and three-minute songs.</p>

## Output

<p>For each test case print the minimal possible difference in minutes between the concerts durations.</p>





```input1
4
1 1 1
2 1 3
5 5 5
1 1 2
```




```output1
0
1
0
1
```



## Note

<p>In the first test case, Luntik can include a one-minute song and a two-minute song into the first concert, and a three-minute song into the second concert. Then the difference will be equal to $0$.</p><p>In the second test case, Luntik can include two one-minute songs and a two-minute song and a three-minute song into the first concert, and two three-minute songs into the second concert. The duration of the first concert will be $1 + 1 + 2 + 3 = 7$, the duration of the second concert will be $6$. The difference of them is $|7-6| = 1$.</p>
