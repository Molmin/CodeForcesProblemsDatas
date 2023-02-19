## Description

<div><p>Little09 and his friends are playing a game. There are $n$ players, and the temperature value of the player $i$ is $i$. </p><p>The types of environment are expressed as $0$ or $1$. When two players fight in a specific environment, if its type is $0$, the player with a lower temperature value in this environment always wins; if it is $1$, the player with a higher temperature value in this environment always wins. The types of the $n-1$ environments form a binary string $s$ with a length of $n-1$.</p><p>If there are $x$ players participating in the game, there will be a total of $x-1$ battles, and the types of the $x-1$ environments will be the first $x-1$ characters of $s$. While there is more than one player left in the tournament, choose any two remaining players to fight. The player who loses will be eliminated from the tournament. The type of the environment of battle $i$ is $s_i$.</p><p>For each $x$ from $2$ to $n$, answer the following question: if all players whose temperature value does not exceed $x$ participate in the game, how many players have a chance to win?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\le t \le 10^3$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 2\cdot 10^5$) &nbsp;— the number of players.</p><p>The second line of each test case contains a binary string $s$ with a length $n-1$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output $n-1$ integers &nbsp;— for each $x$ from $2$ to $n$, output the number of players that have a chance to win.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1\le t \le 10^3$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\leq n\leq 2\cdot 10^5$) &nbsp;— the number of players.</p><p>The second line of each test case contains a binary string $s$ with a length $n-1$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3\cdot 10^5$.</p>

## Output

<p>For each test case output $n-1$ integers &nbsp;— for each $x$ from $2$ to $n$, output the number of players that have a chance to win.</p>





```input1|2,3
2
4
001
4
101
```




```output1
1 1 3 
1 2 3
```



## Note

<p>In the first test case, for $x=2$ and $x=3$, only the player whose temperature value is $1$ can be the winner. For $x=4$, the player whose temperature value is $2,3,4$ can be the winner.</p>
