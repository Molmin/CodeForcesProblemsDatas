## Description

<div><p>Marian is at a casino. The game at the casino works like this.</p><p>Before each round, the player selects a number between $1$ and $10^9$. After that, a dice with $10^9$ faces is rolled so that a random number between $1$ and $10^9$ appears. If the player guesses the number correctly their total money is doubled, else their total money is halved. </p><p>Marian predicted the future and knows all the numbers $x_1, x_2, \dots, x_n$ that the dice will show in the next $n$ rounds. </p><p>He will pick three integers $a$, $l$ and $r$ ($l \leq r$). He will play $r-l+1$ rounds (rounds between $l$ and $r$ inclusive). In each of these rounds, he will guess the same number $a$. At the start (before the round $l$) he has $1$ dollar.</p><p>Marian asks you to determine the integers $a$, $l$ and $r$ ($1 \leq a \leq 10^9$, $1 \leq l \leq r \leq n$) such that he makes the most money at the end.</p><p>Note that during halving and multiplying there is no rounding and there are no precision errors. So, for example during a game, Marian could have money equal to $\dfrac{1}{1024}$, $\dfrac{1}{128}$, $\dfrac{1}{2}$, $1$, $2$, $4$, etc. (any value of $2^t$, where $t$ is an integer of any sign).</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot 10^5$)&nbsp;— the number of rounds.</p><p>The second line of each test case contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \leq x_i \leq 10^9$), where $x_i$ is the number that will fall on the dice in the $i$-th round.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, output three integers $a$, $l$, and $r$ such that Marian makes the most amount of money gambling with his strategy. If there are multiple answers, you may output any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 2\cdot 10^5$)&nbsp;— the number of rounds.</p><p>The second line of each test case contains $n$ integers $x_1, x_2, \dots, x_n$ ($1 \leq x_i \leq 10^9$), where $x_i$ is the number that will fall on the dice in the $i$-th round.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, output three integers $a$, $l$, and $r$ such that Marian makes the most amount of money gambling with his strategy. If there are multiple answers, you may output any of them.</p>





```input1|2,3,6,7
4
5
4 4 3 4 4
5
11 1 11 1 11
1
1000000000
10
8 8 8 9 9 6 6 9 6 6
```




```output1
4 1 5
1 2 2
1000000000 1 1
6 6 10
```



## Note

<p>For the first test case, the best choice is $a=4$, $l=1$, $r=5$, and the game would go as follows. </p><ul> <li> Marian starts with one dollar. </li><li> After the first round, he ends up with $2$ dollars because the numbers coincide with the chosen one. </li><li> After the second round, he ends up with $4$ dollars because the numbers coincide again. </li><li> After the third round, he ends up with $2$ dollars because he guesses $4$ even though $3$ is the correct choice. </li><li> After the fourth round, he ends up with $4$ dollars again. </li><li> In the final round, he ends up $8$ dollars because he again guessed correctly. </li></ul><p>There are many possible answers for the second test case, but it can be proven that Marian will not end up with more than $2$ dollars, so any choice with $l = r$ with the appropriate $a$ is acceptable.</p>
