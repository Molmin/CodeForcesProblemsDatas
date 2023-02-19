## Description

<div><p><span class="tex-font-style-bf">The only difference between the easy and hard versions are the locations you can teleport to.</span></p><p>Consider the points $0, 1, \dots, n$ on the number line. There is a teleporter located on each of the points $1, 2, \dots, n$. At point $i$, you can do the following:</p><ul> <li> Move left one unit: it costs $1$ coin. </li><li> Move right one unit: it costs $1$ coin. </li><li> Use a teleporter at point $i$, if it exists: it costs $a_i$ coins. As a result, you teleport to point $0$. Once you use a teleporter, you <span class="tex-font-style-bf">can't</span> use it again. </li></ul><p>You have $c$ coins, and you start at point $0$. What's the most number of teleporters you can use?</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$ and $c$ ($1 \leq n \leq 2\cdot10^5$; $1 \leq c \leq 10^9$) &nbsp;— the length of the array and the number of coins you have respectively.</p><p>The following line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the costs to use the teleporters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum number of teleporters you can use.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. The descriptions of the test cases follow.</p><p>The first line of each test case contains two integers $n$ and $c$ ($1 \leq n \leq 2\cdot10^5$; $1 \leq c \leq 10^9$) &nbsp;— the length of the array and the number of coins you have respectively.</p><p>The following line contains $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the costs to use the teleporters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output the maximum number of teleporters you can use.</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
5 6
1 1 1 1 1
8 32
100 52 13 6 9 4 100 35
1 1
5
4 5
4 3 2 1
5 9
2 3 1 4 1
5 8
2 3 1 4 1
4 3
2 3 4 1
4 9
5 4 3 3
2 14
7 5
5 600000000
500000000 400000000 300000000 200000000 100000000
```




```output1
2
2
0
1
2
2
1
1
1
2
```



## Note

<p>In the first test case, you can move one unit to the right, use the teleporter at index $1$ and teleport to point $0$, move two units to the right and use the teleporter at index $2$. You are left with $6-1-1-2-1 = 1$ coins you don't have enough coins to use another teleporter. You have used two teleporters, so the answer is two.</p><p>In the second test case, you go four units to the right and use the teleporter to go to $0$, then go six units right and use the teleporter at index $6$ to go to $0$. The total cost will be $4+6+6+4 = 20$. You are left with $12$ coins, but it is not enough to reach any other teleporter and use it so the answer is $2$.</p><p>In the third test case, you don't have enough coins to use any teleporter, so the answer is zero.</p>
