## Description

<div><p>There are $n$ athletes in front of you. Athletes are numbered from $1$ to $n$ from left to right. You know the strength of each athlete&nbsp;— the athlete number $i$ has the strength $s_i$.</p><p>You want to split all athletes into two teams. Each team must have at least one athlete, and each athlete must be exactly in one team.</p><p>You want the strongest athlete from the first team to differ as little as possible from the weakest athlete from the second team. Formally, you want to split the athletes into two teams $A$ and $B$ so that the value $|\max(A) - \min(B)|$ is as small as possible, where $\max(A)$ is the maximum strength of an athlete from team $A$, and $\min(B)$ is the minimum strength of an athlete from team $B$.</p><p>For example, if $n=5$ and the strength of the athletes is $s=[3, 1, 2, 6, 4]$, then one of the possible split into teams is: </p><ul> <li> first team: $A = [1, 2, 4]$, </li><li> second team: $B = [3, 6]$. </li></ul><p>In this case, the value $|\max(A) - \min(B)|$ will be equal to $|4-3|=1$. This example illustrates one of the ways of optimal split into two teams.</p><p>Print the minimum value $|\max(A) - \min(B)|$.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case consists of two lines. </p><p>The first line contains positive integer $n$ ($2 \le n \le 50$)&nbsp;— number of athletes. </p><p>The second line contains $n$ positive integers $s_1, s_2, \ldots, s_n$ ($1 \le s_i \le 1000$), where $s_i$&nbsp;— is the strength of the $i$-th athlete. Please note that $s$ values may not be distinct.</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the minimum value of $|\max(A) - \min(B)|$ with the optimal split of all athletes into two teams. Each of the athletes must be a member of exactly one of the two teams.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case consists of two lines. </p><p>The first line contains positive integer $n$ ($2 \le n \le 50$)&nbsp;— number of athletes. </p><p>The second line contains $n$ positive integers $s_1, s_2, \ldots, s_n$ ($1 \le s_i \le 1000$), where $s_i$&nbsp;— is the strength of the $i$-th athlete. Please note that $s$ values may not be distinct.</p>

## Output

<p>For each test case print one integer&nbsp;— the minimum value of $|\max(A) - \min(B)|$ with the optimal split of all athletes into two teams. Each of the athletes must be a member of exactly one of the two teams.</p>





```input1
5
5
3 1 2 6 4
6
2 1 3 2 4 3
4
7 9 3 1
2
1 1000
3
100 150 200
```




```output1
1
0
2
999
50
```



## Note

<p>The first test case was explained in the statement. In the second test case, one of the optimal splits is $A=[2, 1]$, $B=[3, 2, 4, 3]$, so the answer is $|2-2|=0$.</p>
