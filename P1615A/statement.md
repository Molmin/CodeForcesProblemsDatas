## Description

<div><p>There are $n$ block towers in a row, where tower $i$ has a height of $a_i$. You're part of a building crew, and you want to make the buildings look as nice as possible. In a single day, you can perform the following operation:</p><ul> <li> Choose two indices $i$ and $j$ ($1 \leq i, j \leq n$; $i \neq j$), and move a block from tower $i$ to tower $j$. This essentially decreases $a_i$ by $1$ and increases $a_j$ by $1$. </li></ul><p>You think the ugliness of the buildings is the height difference between the tallest and shortest buildings. Formally, the ugliness is defined as $\max(a)-\min(a)$. </p><p>What's the minimum possible ugliness you can achieve, after any number of days?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 100$)&nbsp;— the number of buildings.</p><p>The second line of each test case contains $n$ space separated integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^7$)&nbsp;— the heights of the buildings.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum possible ugliness of the buildings.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 100$)&nbsp;— the number of buildings.</p><p>The second line of each test case contains $n$ space separated integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^7$)&nbsp;— the heights of the buildings.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum possible ugliness of the buildings.</p>





```input1
3
3
10 10 10
4
3 2 1 2
5
1 2 3 1 5
```




```output1
0
0
1
```



## Note

<p>In the first test case, the ugliness is already $0$.</p><p>In the second test case, you should do one operation, with $i = 1$ and $j = 3$. The new heights will now be $[2, 2, 2, 2]$, with an ugliness of $0$.</p><p>In the third test case, you may do three operations: </p><ol> <li> with $i = 3$ and $j = 1$. The new array will now be $[2, 2, 2, 1, 5]$, </li><li> with $i = 5$ and $j = 4$. The new array will now be $[2, 2, 2, 2, 4]$, </li><li> with $i = 5$ and $j = 3$. The new array will now be $[2, 2, 3, 2, 3]$. </li></ol> The resulting ugliness is $1$. It can be proven that this is the minimum possible ugliness for this test.
