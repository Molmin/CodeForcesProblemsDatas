## Description

<div><p>Highway 201 is the most busy street in Rockport. Traffic cars cause a lot of hindrances to races, especially when there are a lot of them. The track which passes through this highway can be divided into $n$ sub-tracks. You are given an array $a$ where $a_i$ represents the number of traffic cars in the $i$-th sub-track. You define the inconvenience of the track as $\sum\limits_{i=1}^{n} \sum\limits_{j=i+1}^{n} \lvert a_i-a_j\rvert$, where $|x|$ is the absolute value of $x$. </p><p>You can perform the following operation any (possibly zero) number of times: choose a traffic car and move it from its current sub-track to any other sub-track.</p><p>Find the minimum inconvenience you can achieve.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1\leq t\leq 10\,000$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 2\cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0\leq a_i\leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line containing a single integer: the minimum inconvenience you can achieve by applying the given operation any (possibly zero) number of times.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1\leq t\leq 10\,000$) — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1\leq n\leq 2\cdot 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0\leq a_i\leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, print a single line containing a single integer: the minimum inconvenience you can achieve by applying the given operation any (possibly zero) number of times.</p>





```input1
3
3
1 2 3
4
0 1 1 0
10
8 3 6 11 5 2 1 7 10 4
```




```output1
0
4
21
```



## Note

<p>For the first test case, you can move a car from the $3$-rd sub-track to the $1$-st sub-track to obtain $0$ inconvenience.</p><p>For the second test case, moving any car won't decrease the inconvenience of the track.</p>
