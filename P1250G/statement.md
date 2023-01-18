## Description

<div><p>Eulampius has created a game with the following rules:</p><ul><li> there are two players in the game: a human and a computer; </li><li> the game lasts for no more than $n$ rounds. Initially both players have $0$ points. In the $j$-th round the human gains $a_j$ points, and the computer gains $b_j$ points. The points are gained simultaneously;</li><li> the game ends when one of the players gets $k$ or more points. This player loses the game. If both players get $k$ or more points simultaneously, both lose;</li><li> if both players have less than $k$ points after $n$ rounds, the game ends in a tie;</li><li> after each round the human can push the "Reset" button. If the human had $x$ points, and the computer had $y$ points before the button is pushed (of course, $x &lt; k$ and $y &lt; k$), then after the button is pushed the human will have $x' = max(0, \, x - y)$ points, and the computer will have $y' = max(0, \, y - x)$ points. E. g. the push of "Reset" button transforms the state $(x=3, \, y=5)$ into the state $(x'=0, \, y'=2)$, and the state $(x=8, \, y=2)$ into the state $(x'=6, \, y'=0)$.</li></ul><p>Eulampius asked his friend Polycarpus to test the game. Polycarpus has quickly revealed that amounts of points gained by the human and the computer in each of $n$ rounds are generated before the game and stored in a file. In other words, the pushes of the "Reset" button do not influence the values $a_j$ and $b_j$, so sequences $a$ and $b$ are fixed and known in advance.</p><p>Polycarpus wants to make a plan for the game. He would like to win the game pushing the "Reset" button as few times as possible. Your task is to determine this minimal number of pushes or determine that Polycarpus cannot win.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10000$)&nbsp;— the number of test cases. Then the test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $2 \le k \le 10^9$)&nbsp;— the maximum possible number of rounds in the game and the number of points, after reaching which a player loses, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_j &lt; k)$, where $a_j$ is the amount of points the human gains in the $j$-th round.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_j &lt; k$), where $b_j$ is the amount of points the computer gains in the $j$-th round.</p><p>The sum of $n$ over all test cases in the input does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Print the answers for all test cases in the order they appear in the input.</p><p>If Polycarpus cannot win the game, then simply print one line "<span class="tex-font-style-tt">-1</span>" (without quotes). In this case, you should not output anything else for that test case. Otherwise, the first line of the test case answer should contain one integer $d$&nbsp;— the minimum possible number of "Reset" button pushes, required to win the game. The next line should contain $d$ distinct integers $r_1, r_2, \dots, r_d$ ($1 \le r_i &lt; n$)&nbsp;— the numbers of rounds, at the end of which Polycarpus has to press the "Reset" button, in arbitrary order. If $d=0$ then either leave the second line of the test case answer empty, or do not print the second line at all.</p><p>If there are several possible solutions, print any of them.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10000$)&nbsp;— the number of test cases. Then the test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n \le 2 \cdot 10^5$, $2 \le k \le 10^9$)&nbsp;— the maximum possible number of rounds in the game and the number of points, after reaching which a player loses, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_j &lt; k)$, where $a_j$ is the amount of points the human gains in the $j$-th round.</p><p>The third line of each test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_j &lt; k$), where $b_j$ is the amount of points the computer gains in the $j$-th round.</p><p>The sum of $n$ over all test cases in the input does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Print the answers for all test cases in the order they appear in the input.</p><p>If Polycarpus cannot win the game, then simply print one line "<span class="tex-font-style-tt">-1</span>" (without quotes). In this case, you should not output anything else for that test case. Otherwise, the first line of the test case answer should contain one integer $d$&nbsp;— the minimum possible number of "Reset" button pushes, required to win the game. The next line should contain $d$ distinct integers $r_1, r_2, \dots, r_d$ ($1 \le r_i &lt; n$)&nbsp;— the numbers of rounds, at the end of which Polycarpus has to press the "Reset" button, in arbitrary order. If $d=0$ then either leave the second line of the test case answer empty, or do not print the second line at all.</p><p>If there are several possible solutions, print any of them.</p>





```input1
3
4 17
1 3 5 7
3 5 7 9
11 17
5 2 8 2 4 6 1 2 7 2 5
4 6 3 3 5 1 7 4 2 5 3
6 17
6 1 2 7 2 5
1 7 4 2 5 3
```




```output1
0

2
2 4
-1
```



## Note

<p>In the second test case, if the human pushes the "Reset" button after the second and the fourth rounds, the game goes as follows:</p><ol> <li> after the first round the human has $5$ points, the computer&nbsp;— $4$ points; </li><li> after the second round the human has $7$ points, the computer&nbsp;— $10$ points; </li><li> the human pushes the "Reset" button and now he has $0$ points and the computer&nbsp;— $3$ points; </li><li> after the third round the human has $8$ points, the computer&nbsp;— $6$ points; </li><li> after the fourth round the human has $10$ points, the computer&nbsp;— $9$ points; </li><li> the human pushes "Reset" button again, after it he has $1$ point, the computer&nbsp;— $0$ points; </li><li> after the fifth round the human has $5$ points, the computer&nbsp;— $5$ points; </li><li> after the sixth round the human has $11$ points, the computer&nbsp;— $6$ points; </li><li> after the seventh round the human has $12$ points, the computer&nbsp;— $13$ points; </li><li> after the eighth round the human has $14$ points, the computer&nbsp;— $17$ points; </li><li> the human wins, as the computer has $k$ or more points and the human&nbsp;— strictly less than $k$ points. </li></ol>
