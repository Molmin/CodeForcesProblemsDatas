## Description

<div><p>So the Beautiful Regional Contest (BeRC) has come to an end! $n$ students took part in the contest. The final standings are already known: the participant in the $i$-th place solved $p_i$ problems. Since the participants are primarily sorted by the number of solved problems, then $p_1 \ge p_2 \ge \dots \ge p_n$.</p><p>Help the jury distribute the gold, silver and bronze medals. Let their numbers be $g$, $s$ and $b$, respectively. Here is a list of requirements from the rules, which all must be satisfied:</p><ul> <li> for each of the three types of medals, at least one medal must be awarded (that is, $g&gt;0$, $s&gt;0$ and $b&gt;0$); </li><li> the number of gold medals must be strictly less than the number of silver and the number of bronze (that is, $g&lt;s$ and $g&lt;b$, but there are no requirements between $s$ and $b$); </li><li> each gold medalist must solve strictly more problems than any awarded with a silver medal; </li><li> each silver medalist must solve strictly more problems than any awarded a bronze medal; </li><li> each bronze medalist must solve strictly more problems than any participant not awarded a medal; </li><li> the total number of medalists $g+s+b$ should not exceed half of all participants (for example, if $n=21$, then you can award a maximum of $10$ participants, and if $n=26$, then you can award a maximum of $13$ participants). </li></ul><p>The jury wants to reward with medals the total <span class="tex-font-style-bf">maximal</span> number participants (i.e. to maximize $g+s+b$) so that all of the items listed above are fulfilled. Help the jury find such a way to award medals.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 10000$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of a test case contains an integer $n$ ($1 \le n \le 4\cdot10^5$) — the number of BeRC participants. The second line of a test case contains integers $p_1, p_2, \dots, p_n$ ($0 \le p_i \le 10^6$), where $p_i$ is equal to the number of problems solved by the $i$-th participant from the final standings. The values $p_i$ are sorted in non-increasing order, i.e. $p_1 \ge p_2 \ge \dots \ge p_n$.</p><p>The sum of $n$ over all test cases in the input does not exceed $4\cdot10^5$.</p></div><div class="output-specification"><p>Print $t$ lines, the $j$-th line should contain the answer to the $j$-th test case.</p><p>The answer consists of three non-negative integers $g, s, b$.</p><ul> <li> Print $g=s=b=0$ if there is no way to reward participants with medals so that all requirements from the statement are satisfied at the same time. </li><li> Otherwise, print three positive numbers $g, s, b$ — the possible number of gold, silver and bronze medals, respectively. The sum of $g+s+b$ should be the maximum possible. If there are several answers, print any of them. </li></ul></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 10000$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of a test case contains an integer $n$ ($1 \le n \le 4\cdot10^5$) — the number of BeRC participants. The second line of a test case contains integers $p_1, p_2, \dots, p_n$ ($0 \le p_i \le 10^6$), where $p_i$ is equal to the number of problems solved by the $i$-th participant from the final standings. The values $p_i$ are sorted in non-increasing order, i.e. $p_1 \ge p_2 \ge \dots \ge p_n$.</p><p>The sum of $n$ over all test cases in the input does not exceed $4\cdot10^5$.</p>

## Output

<p>Print $t$ lines, the $j$-th line should contain the answer to the $j$-th test case.</p><p>The answer consists of three non-negative integers $g, s, b$.</p><ul> <li> Print $g=s=b=0$ if there is no way to reward participants with medals so that all requirements from the statement are satisfied at the same time. </li><li> Otherwise, print three positive numbers $g, s, b$ — the possible number of gold, silver and bronze medals, respectively. The sum of $g+s+b$ should be the maximum possible. If there are several answers, print any of them. </li></ul>





```input1
5
12
5 4 4 3 2 2 1 1 1 1 1 1
4
4 3 2 1
1
1000000
20
20 19 18 17 16 15 14 13 12 11 10 9 8 7 6 5 4 3 2 1
32
64 64 63 58 58 58 58 58 37 37 37 37 34 34 28 28 28 28 28 28 24 24 19 17 17 17 17 16 16 16 16 11
```




```output1
1 2 3
0 0 0
0 0 0
2 5 3
2 6 6
```



## Note

<p>In the first test case, it is possible to reward $1$ gold, $2$ silver and $3$ bronze medals. In this case, the participant solved $5$ tasks will be rewarded with the gold medal, participants solved $4$ tasks will be rewarded with silver medals, participants solved $2$ or $3$ tasks will be rewarded with bronze medals. Participants solved exactly $1$ task won't be rewarded. It's easy to see, that in this case, all conditions are satisfied and it is possible to reward participants in this way. It is impossible to give more than $6$ medals because the number of medals should not exceed half of the number of participants. The answer $1$, $3$, $2$ is also correct in this test case.</p><p>In the second and third test cases, it is impossible to reward medals, because at least one medal of each type should be given, but the number of medals should not exceed half of the number of participants.</p>
