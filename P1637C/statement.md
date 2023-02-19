## Description

<div><p>Andrew has $n$ piles with stones. The $i$-th pile contains $a_i$ stones. He wants to make his table clean so he decided to put every stone either to the $1$-st or the $n$-th pile.</p><p>Andrew can perform the following operation any number of times: choose $3$ indices $1 \le i &lt; j &lt; k \le n$, such that the $j$-th pile contains at least $2$ stones, then he takes $2$ stones from the pile $j$ and puts one stone into pile $i$ and one stone into pile $k$. </p><p>Tell Andrew what is the minimum number of operations needed to move all the stones to piles $1$ and $n$, or determine if it's impossible.</p></div><div class="input-specification"><p>The input contains several test cases. The first line contains one integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;— the number of test cases.</p><p>The first line for each test case contains one integer $n$ ($3 \leq n \leq 10^5$)&nbsp;— the length of the array.</p><p>The second line contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the array elements.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print the minimum number of operations needed to move stones to piles $1$ and $n$, or print $-1$ if it's impossible.</p></div>

## Input

<p>The input contains several test cases. The first line contains one integer $t$ ($1 \leq t \leq 10\,000$)&nbsp;— the number of test cases.</p><p>The first line for each test case contains one integer $n$ ($3 \leq n \leq 10^5$)&nbsp;— the length of the array.</p><p>The second line contains a sequence of integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$)&nbsp;— the array elements.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print the minimum number of operations needed to move stones to piles $1$ and $n$, or print $-1$ if it's impossible.</p>





```input1
4
5
1 2 2 3 6
3
1 3 1
3
1 2 1
4
3 1 1 2
```




```output1
4
-1
1
-1
```



## Note

<p>In the first test case, it is optimal to do the following: </p><ol> <li> Select $(i, j, k) = (1, 2, 5)$. The array becomes equal to $[2, 0, 2, 3, 7]$. </li><li> Select $(i, j, k) = (1, 3, 4)$. The array becomes equal to $[3, 0, 0, 4, 7]$. </li><li> Twice select $(i, j, k) = (1, 4, 5)$. The array becomes equal to $[5, 0, 0, 0, 9]$. This array satisfy the statement, because every stone is moved to piles $1$ and $5$. </li></ol> There are $4$ operations in total.<p>In the second test case, it's impossible to put all stones into piles with numbers $1$ and $3$: </p><ol> <li> At the beginning there's only one possible operation with $(i, j, k) = (1, 2, 3)$. The array becomes equal to $[2, 1, 2]$. </li><li> Now there is no possible operation and the array doesn't satisfy the statement, so the answer is $-1$. </li></ol><p>In the third test case, it's optimal to do the following: </p><ol> <li> Select $(i, j, k) = (1, 2, 3)$. The array becomes equal to $[2, 0, 2]$. This array satisfies the statement, because every stone is moved to piles $1$ and $3$. </li></ol> The is $1$ operation in total.<p>In the fourth test case, it's impossible to do any operation, and the array doesn't satisfy the statement, so the answer is $-1$.</p>
