## Description

<div><p>There is a badminton championship in which $n$ players take part. The players are numbered from $1$ to $n$. </p><p>The championship proceeds as follows: player $1$ and player $2$ play a game, then the winner and player $3$ play a game, and then the winner and player $4$ play a game, and so on. So, $n-1$ games are played, and the winner of the last game becomes the champion. There are no draws in the games.</p><p>You want to find out the result of championship. Currently, you only know the following information:</p><ul> <li> Each player has either won $x$ games or $y$ games in the championship. </li></ul><p>Given $n$, $x$, and $y$, find out if there is a result that matches this information.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains three integers $n$, $x$, $y$ ($2 \le n \le 10^5$, $0 \le x, y &lt; n$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print the answer for each test case, one per line. If there is no result that matches the given information about $n$, $x$, $y$, print $-1$. Otherwise, print $n-1$ space separated integers, where the $i$-th integer is the player number of the winner of the $i$-th game. </p><p>If there are multiple valid results, print any.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains three integers $n$, $x$, $y$ ($2 \le n \le 10^5$, $0 \le x, y &lt; n$).</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>Print the answer for each test case, one per line. If there is no result that matches the given information about $n$, $x$, $y$, print $-1$. Otherwise, print $n-1$ space separated integers, where the $i$-th integer is the player number of the winner of the $i$-th game. </p><p>If there are multiple valid results, print any.</p>





```input1|2,4,6
5
5 2 0
8 1 2
3 0 0
2 0 1
6 3 0
```




```output1
1 1 4 4
-1
-1
2 
-1
```



## Note

<p>In the first test case, player $1$ and player $4$ won $x$ times, player $2$ and player $3$ won $y$ times.</p><p>In the second, third, and fifth test cases, no valid result exists.</p>
