## Description

<div><p>You are given an integer $n$. In $1$ move, you can do one of the following actions:</p><ul> <li> erase any digit of the number (it's acceptable that the number before the operation has exactly one digit and after the operation, it is "empty"); </li><li> add one digit <span class="tex-font-style-bf">to the right</span>. </li></ul><p>The actions may be performed in any order any number of times.</p><p>Note that if, after deleting some digit from a number, it will contain leading zeroes, they will <span class="tex-font-style-bf">not</span> be deleted. E.g. if you delete from the number $301$ the digit $3$, the result is the number $01$ (not $1$).</p><p>You need to perform the <span class="tex-font-style-bf">minimum</span> number of actions to make the number any power of $2$ (i.e. there's an integer $k$ ($k \ge 0$) such that the resulting number is equal to $2^k$). <span class="tex-font-style-bf">The resulting number must not have leading zeroes</span>.</p><p>E.g. consider $n=1052$. The answer is equal to $2$. First, let's add to the right one digit $4$ (the result will be $10524$). Then let's erase the digit $5$, so the result will be $1024$ which is a power of $2$.</p><p>E.g. consider $n=8888$. The answer is equal to $3$. Let's erase any of the digits $8$ three times. The result will be $8$ which is a power of $2$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, output in a separate line one integer $m$ — the minimum number of moves to transform the number into any power of $2$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 10^9$).</p>

## Output

<p>For each test case, output in a separate line one integer $m$ — the minimum number of moves to transform the number into any power of $2$.</p>





```input1
12
1052
8888
6
75
128
1
301
12048
1504
6656
1000000000
687194767
```




```output1
2
3
1
3
0
0
2
1
3
4
9
2
```



## Note

<p>The answer for the first test case was considered above.</p><p>The answer for the second test case was considered above.</p><p>In the third test case, it's enough to add to the right the digit $4$ — the number $6$ will turn into $64$.</p><p>In the fourth test case, let's add to the right the digit $8$ and then erase $7$ and $5$ — the taken number will turn into $8$.</p><p>The numbers of the fifth and the sixth test cases are already powers of two so there's no need to make any move.</p><p>In the seventh test case, you can delete first of all the digit $3$ (the result is $01$) and then the digit $0$ (the result is $1$).</p>
