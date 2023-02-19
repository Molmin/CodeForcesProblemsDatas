## Description

<div><p>There are $n$ traps numbered from $1$ to $n$. You will go through them one by one in order. The $i$-th trap deals $a_i$ base damage to you.</p><p>Instead of going through a trap, you can jump it over. You can jump over no more than $k$ traps. If you jump over a trap, it does not deal any damage to you. But there is an additional rule: if you jump over a trap, all next traps damages increase by $1$ (this is a bonus damage).</p><p>Note that if you jump over a trap, you don't get any damage (neither base damage nor bonus damage). Also, the bonus damage stacks so, for example, if you go through a trap $i$ with base damage $a_i$, and you have already jumped over $3$ traps, you get $(a_i + 3)$ damage.</p><p>You have to find the minimal damage that it is possible to get if you are allowed to jump over no more than $k$ traps.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le k \le n$)&nbsp;— the number of traps and the number of jump overs that you are allowed to make.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— base damage values of all traps.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output a single integer — the minimal total damage that it is possible to get if you are allowed to jump over no more than $k$ traps.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $1 \le k \le n$)&nbsp;— the number of traps and the number of jump overs that you are allowed to make.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— base damage values of all traps.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output a single integer — the minimal total damage that it is possible to get if you are allowed to jump over no more than $k$ traps.</p>





```input1|2,3,6,7,10,11
5
4 4
8 7 1 4
4 1
5 10 11 5
7 5
8 2 5 15 11 2 8
6 3
1 2 3 4 5 6
1 1
7
```




```output1
0
21
9
6
0
```



## Note

<p>In the first test case it is allowed to jump over all traps and take $0$ damage.</p><p>In the second test case there are $5$ ways to jump over some traps:</p><ol> <li> Do not jump over any trap.<p>Total damage: $5 + 10 + 11 + 5 = 31$.</p></li><li> Jump over the $1$-st trap.<p>Total damage: $\underline{0} + (10 + 1) + (11 + 1) + (5 + 1) = 29$.</p></li><li> Jump over the $2$-nd trap.<p>Total damage: $5 + \underline{0} + (11 + 1) + (5 + 1) = 23$.</p></li><li> Jump over the $3$-rd trap.<p>Total damage: $5 + 10 + \underline{0} + (5 + 1) = 21$.</p></li><li> Jump over the $4$-th trap.<p>Total damage: $5 + 10 + 11 + \underline{0} = 26$.</p></li></ol><p>To get minimal damage it is needed to jump over the $3$-rd trap, so the answer is $21$.</p><p>In the third test case it is optimal to jump over the traps $1$, $3$, $4$, $5$, $7$:</p><p>Total damage: $0 + (2 + 1) + 0 + 0 + 0 + (2 + 4) + 0 = 9$.</p>
