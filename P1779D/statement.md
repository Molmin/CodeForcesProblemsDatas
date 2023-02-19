## Description

<div><p>Boris thinks that chess is a tedious game. So he left his tournament early and went to a barber shop as his hair was a <span class="tex-font-style-it">bit</span> messy.</p><p>His current hair can be described by an array $a_1,a_2,\ldots, a_n$, where $a_i$ is the height of the hair standing at position $i$. His desired haircut can be described by an array $b_1,b_2,\ldots, b_n$ in a similar fashion.</p><p>The barber has $m$ razors. Each has its own size and can be used <span class="tex-font-style-bf">at most</span> once. In one operation, he chooses a razor and cuts a segment of Boris's hair. More formally, an operation is:</p><ul> <li> Choose any razor which hasn't been used before, let its size be $x$; </li><li> Choose a segment $[l,r]$ ($1\leq l \leq r \leq n$); </li><li> Set $a_i := \min (a_i,x)$ for each $l\leq i \leq r$; </li></ul><p>Notice that some razors might have equal sizes&nbsp;— the barber can choose some size $x$ only as many times as the number of razors with size $x$. </p><p>He may perform as many operations as he wants, as long as any razor is used at most once and $a_i = b_i$ for each $1 \leq i \leq n$ at the end. He <span class="tex-font-style-bf">does not</span> have to use all razors.</p><p>Can you determine whether the barber can give Boris his desired haircut?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 20\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a positive integer $n$ ($3\leq n\leq 2\cdot 10^5$)&nbsp;— the length of arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) &nbsp;— Boris's current hair.</p><p>The third line of each test case contains $n$ positive integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^9$) &nbsp;— Boris's desired hair.</p><p>The fourth line of each test case contains a positive integer $m$ ($1 \leq m \leq 2\cdot 10^5$) &nbsp;— the number of razors.</p><p>The fifth line of each test case contains $m$ positive integers $x_1,x_2, \ldots, x_m$ ($1 \leq x_i \leq 10^9$) &nbsp;— the sizes of the razors.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all test cases do not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if the barber can cut Boris's hair as desired. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "yEs", "yes", "Yes", and "YES" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \leq t \leq 20\,000$). The description of the test cases follows.</p><p>The first line of each test case contains a positive integer $n$ ($3\leq n\leq 2\cdot 10^5$)&nbsp;— the length of arrays $a$ and $b$.</p><p>The second line of each test case contains $n$ positive integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) &nbsp;— Boris's current hair.</p><p>The third line of each test case contains $n$ positive integers $b_1, b_2, \ldots, b_n$ ($1 \leq b_i \leq 10^9$) &nbsp;— Boris's desired hair.</p><p>The fourth line of each test case contains a positive integer $m$ ($1 \leq m \leq 2\cdot 10^5$) &nbsp;— the number of razors.</p><p>The fifth line of each test case contains $m$ positive integers $x_1,x_2, \ldots, x_m$ ($1 \leq x_i \leq 10^9$) &nbsp;— the sizes of the razors.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all test cases do not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if the barber can cut Boris's hair as desired. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can output the answer in any case (upper or lower). For example, the strings "yEs", "yes", "Yes", and "YES" will be recognized as positive responses.</p>





```input1|2,3,4,5,6,12,13,14,15,16,22,23,24,25,26,32,33,34,35,36
7
3
3 3 3
2 1 2
2
1 2
6
3 4 4 6 3 4
3 1 2 3 2 3
3
3 2 3
10
1 2 3 4 5 6 7 8 9 10
1 2 3 4 5 6 7 8 9 10
10
1 2 3 4 5 6 7 8 9 10
3
1 1 1
1 1 2
12
4 2 4 3 1 5 6 3 5 6 2 1
13
7 9 4 5 3 3 3 6 8 10 3 2 5
5 3 1 5 3 2 2 5 8 5 1 1 5
8
1 5 3 5 4 2 3 1
13
7 9 4 5 3 3 3 6 8 10 3 2 5
5 3 1 5 3 2 2 5 8 5 1 1 5
7
1 5 3 4 2 3 1
3
19747843 2736467 938578397
2039844 2039844 2039844
1
2039844
```




```output1
YES
NO
YES
NO
YES
NO
YES
```



## Note

<p>In the first test case, Boris's hair is initially $[3,3,3]$. Let us describe a sequence of $2$ operations the barber can perform:</p><ul> <li> The barber uses the razor with size $1$ on the segment $[2,2]$; hence Boris's hair becomes $[3,1,3]$. </li><li> The barber uses the razor with size $2$ on the segment $[1,3]$; hence Boris's hair becomes $[2,1,2]$ which is the desired haircut. </li></ul><p>In the third test case, no operation has to be done since Boris's hair is already as desired.</p><p>In the fourth test case, no cuts will be able to increase the third element in $[1,1,1]$ in a way that the array becomes $[1,1,2]$.</p>
