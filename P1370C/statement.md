## Description

<div><p>Ashishgup and FastestFinger play a game. </p><p>They start with a number $n$ and play in turns. In each turn, a player can make <span class="tex-font-style-bf">any one</span> of the following moves:</p><ul> <li> Divide $n$ by any of its odd divisors greater than $1$. </li><li> Subtract $1$ from $n$ if $n$ is greater than $1$. </li></ul><p>Divisors of a number include the number itself.</p><p>The player who is <span class="tex-font-style-bf">unable to make a move</span> loses the game.</p><p>Ashishgup moves first. Determine the winner of the game if both of them play optimally.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer &nbsp;— $n$ ($1 \leq n \leq 10^9$).</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">Ashishgup</span>" if he wins, and "<span class="tex-font-style-tt">FastestFinger</span>" otherwise (without quotes).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$) &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer &nbsp;— $n$ ($1 \leq n \leq 10^9$).</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">Ashishgup</span>" if he wins, and "<span class="tex-font-style-tt">FastestFinger</span>" otherwise (without quotes).</p>





```input1
7
1
2
3
4
5
6
12
```




```output1
FastestFinger
Ashishgup
Ashishgup
FastestFinger
Ashishgup
FastestFinger
Ashishgup
```



## Note

<p>In the first test case, $n = 1$, Ashishgup cannot make a move. He loses.</p><p>In the second test case, $n = 2$, Ashishgup subtracts $1$ on the first move. Now $n = 1$, FastestFinger cannot make a move, so he loses.</p><p>In the third test case, $n = 3$, Ashishgup divides by $3$ on the first move. Now $n = 1$, FastestFinger cannot make a move, so he loses.</p><p>In the last test case, $n = 12$, Ashishgup divides it by $3$. Now $n = 4$, FastestFinger is forced to subtract $1$, and Ashishgup gets $3$, so he wins by dividing it by $3$.</p>
