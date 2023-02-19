## Description

<div><p>There is a famous olympiad, which has more than a hundred participants. The Olympiad consists of two stages: the elimination stage, and the final stage. At least a hundred participants will advance to the final stage. The elimination stage in turn consists of two contests.</p><p>A result of the elimination stage is the total score in two contests, but, unfortunately, the jury lost the final standings and has only standings for the first and for the second contest separately. </p><p>In each contest, the participants are ranked by their point score in non-increasing order. When two participants have a tie (earned the same score), they are ranked by their passport number (in accordance with local regulations, all passport numbers are distinct). </p><p>In the first contest, the participant on the 100-th place scored $a$ points. Also, the jury checked all participants from the 1-st to the 100-th place (inclusive) in the first contest and found out that all of them have at least $b$ points in the second contest.</p><p>Similarly, for the second contest, the participant on the 100-th place has $c$ points. And the jury checked that all the participants from the 1-st to the 100-th place (inclusive) have at least $d$ points in the first contest.</p><p>After two contests, all participants are ranked by their total score in two contests in non-increasing order. When participants have the same total score, tie-breaking with passport numbers is used. The <span class="tex-font-style-bf">cutoff score</span> to qualify to the final stage is the total score of the participant on the 100-th place.</p><p>Given integers $a$, $b$, $c$, $d$, please help the jury determine the smallest possible value of the cutoff score.</p></div><div class="input-specification"><p>You need to process $t$ test cases.</p><p>The first line contains an integer $t$ ($1 \leq t \leq 3025$)&nbsp;— the number of test cases. Then descriptions of $t$ test cases follow.</p><p>The first line of each test case contains four integers $a$, $b$, $c$, $d$ ($0 \le a,\,b,\,c,\,d \le 9$; $d \leq a$; $b \leq c$). </p><p>One can show that for any test case satisfying the constraints above, there is at least one olympiad scenario possible.</p></div><div class="output-specification"><p>For each test case print a single integer&nbsp;— the smallest possible cutoff score in some olympiad scenario satisfying the given information.</p></div>

## Input

<p>You need to process $t$ test cases.</p><p>The first line contains an integer $t$ ($1 \leq t \leq 3025$)&nbsp;— the number of test cases. Then descriptions of $t$ test cases follow.</p><p>The first line of each test case contains four integers $a$, $b$, $c$, $d$ ($0 \le a,\,b,\,c,\,d \le 9$; $d \leq a$; $b \leq c$). </p><p>One can show that for any test case satisfying the constraints above, there is at least one olympiad scenario possible.</p>

## Output

<p>For each test case print a single integer&nbsp;— the smallest possible cutoff score in some olympiad scenario satisfying the given information.</p>





```input1
2
1 2 2 1
4 8 9 2
```




```output1
3
12
```



## Note

<p>For the first test case, consider the following olympiad scenario: there are $101$ participants in the elimination stage, each having $1$ point for the first contest and $2$ points for the second contest. Hence the total score of the participant on the 100-th place is $3$.</p><p>For the second test case, consider the following olympiad scenario: </p><ul> <li> there are $50$ participants with points $5$ and $9$ for the first and second contest respectively; </li><li> $50$ participants with points $4$ and $8$ for the first and second contest respectively; </li><li> and $50$ participants with points $2$ and $9$ for the first and second contest respectively. </li></ul> Hence the total point score of the participant on the 100-th place is $12$.
