## Description

<div><p>During their New Year holidays, Alice and Bob play the following game using an array $a$ of $n$ integers: </p><ul> <li> Players take turns, Alice moves first. </li><li> Each turn a player chooses any element and removes it from the array. </li><li> If Alice chooses <span class="tex-font-style-bf">even value</span>, then she adds it to her score. If the chosen value is odd, Alice's score does not change. </li><li> Similarly, if Bob chooses <span class="tex-font-style-bf">odd value</span>, then he adds it to his score. If the chosen value is even, then Bob's score does not change. </li></ul><p>If there are no numbers left in the array, then the game ends. The player with the highest score wins. If the scores of the players are equal, then a draw is declared.</p><p>For example, if $n = 4$ and $a = [5, 2, 7, 3]$, then the game could go as follows (there are other options): </p><ul> <li> On the first move, Alice chooses $2$ and get two points. Her score is now $2$. The array $a$ is now $[5, 7, 3]$. </li><li> On the second move, Bob chooses $5$ and get five points. His score is now $5$. The array $a$ is now $[7, 3]$. </li><li> On the third move, Alice chooses $7$ and get no points. Her score is now $2$. The array $a$ is now $[3]$. </li><li> On the last move, Bob chooses $3$ and get three points. His score is now $8$. The array $a$ is empty now. </li><li> Since Bob has more points at the end of the game, he is the winner. </li></ul><p>You want to find out who will win if both players play optimally. <span class="tex-font-style-bf">Note that there may be duplicate numbers in the array</span>.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of elements in the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the array $a$ used to play the game.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">Alice</span>" if Alice wins with the optimal play; </li><li> "<span class="tex-font-style-tt">Bob</span>" if Bob wins with the optimal play; </li><li> "<span class="tex-font-style-tt">Tie</span>", if a tie is declared during the optimal play. </li></ul></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of elements in the array $a$.</p><p>The next line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the array $a$ used to play the game.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output on a separate line: </p><ul> <li> "<span class="tex-font-style-tt">Alice</span>" if Alice wins with the optimal play; </li><li> "<span class="tex-font-style-tt">Bob</span>" if Bob wins with the optimal play; </li><li> "<span class="tex-font-style-tt">Tie</span>", if a tie is declared during the optimal play. </li></ul>





```input1
4
4
5 2 7 3
3
3 2 1
4
2 2 2 2
2
7 8
```




```output1
Bob
Tie
Alice
Alice
```


