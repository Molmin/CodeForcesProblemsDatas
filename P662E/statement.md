## Description

<div><p>Consider a regular Codeforces round consisting of three problems that uses dynamic scoring.</p><p>You are given an almost final scoreboard. For each participant (including yourself), the time of the accepted submission for each of the problems is given. Also, for each solution you already know whether you are able to hack it or not. The only changes in the scoreboard that will happen before the end of the round are your challenges.</p><p>What is the best place you may take at the end?</p><p>More formally, <span class="tex-span"><i>n</i></span> people are participating (including yourself). For any problem, if it was solved by exactly <span class="tex-span"><i>k</i></span> people at the end of the round, the maximum score for this problem is defined as: </p><ol> <li> If <span class="tex-span"><i>n</i> &lt; 2<i>k</i> ≤ 2<i>n</i></span>, then the maximum possible score is <span class="tex-span">500</span>; </li><li> If <span class="tex-span"><i>n</i> &lt; 4<i>k</i> ≤ 2<i>n</i></span>, then the maximum possible score is <span class="tex-span">1000</span>; </li><li> If <span class="tex-span"><i>n</i> &lt; 8<i>k</i> ≤ 2<i>n</i></span>, then the maximum possible score is <span class="tex-span">1500</span>; </li><li> If <span class="tex-span"><i>n</i> &lt; 16<i>k</i> ≤ 2<i>n</i></span>, then the maximum possible score is <span class="tex-span">2000</span>; </li><li> If <span class="tex-span"><i>n</i> &lt; 32<i>k</i> ≤ 2<i>n</i></span>, then the maximum possible score is <span class="tex-span">2500</span>; </li><li> If <span class="tex-span">32<i>k</i> ≤ <i>n</i></span>, then the maximum possible score is <span class="tex-span">3000</span>. </li></ol><p>Let the maximum possible score for some problem be equal to <span class="tex-span"><i>s</i></span>. Then a contestant who didn't manage to get it accepted (or his solution was hacked) earns <span class="tex-span">0</span> points for this problem. If he got the the solution accepted <span class="tex-span"><i>t</i></span> minutes after the beginning of the round (and his solution wasn't hacked), he earns <img align="middle" class="tex-formula" src="file://mD0hb9ph.png" style="max-width: 100.0%;max-height: 100.0%;"> points for this problem.</p><p>The overall score of a participant is equal to the sum of points he earns for each problem plus <span class="tex-span">100</span> points for each successful hack (only you make hacks).</p><p>The resulting place you get is equal to one plus the number of participants who's overall score is strictly greater than yours.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of participants. You are the participant number <span class="tex-span">1</span>.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> means that the participant number <span class="tex-span"><i>i</i></span> didn't manage to accept first problem. If <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 120</span>, then the participant number <span class="tex-span"><i>i</i></span> got the first problem accepted <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> minutes after the start of the contest and you cannot hack this solution. Finally, <span class="tex-span"> - 120 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤  - 1</span> means that the participant number <span class="tex-span"><i>i</i></span> got the first problem accepted <span class="tex-span"> - <i>a</i><sub class="lower-index"><i>i</i></sub></span> minutes after the start of the contest and you can hack this solution. Similarly, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> provide the information regarding second and third problems in the same format.</p><p>It's guaranteed that integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> are non-negative.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the best place you can take at the end of the round.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the number of participants. You are the participant number <span class="tex-span">1</span>.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> means that the participant number <span class="tex-span"><i>i</i></span> didn't manage to accept first problem. If <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 120</span>, then the participant number <span class="tex-span"><i>i</i></span> got the first problem accepted <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> minutes after the start of the contest and you cannot hack this solution. Finally, <span class="tex-span"> - 120 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤  - 1</span> means that the participant number <span class="tex-span"><i>i</i></span> got the first problem accepted <span class="tex-span"> - <i>a</i><sub class="lower-index"><i>i</i></sub></span> minutes after the start of the contest and you can hack this solution. Similarly, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> provide the information regarding second and third problems in the same format.</p><p>It's guaranteed that integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> are non-negative.</p>

## Output

<p>Print the only integer&nbsp;— the best place you can take at the end of the round.</p>





```input1
4
120 120 1
61 61 120
-61 61 120
0 0 0

```




```input2
4
0 0 119
-3 -17 -42
0 7 0
51 0 0

```




```output1
1

```




```output2
2

```



## Note

<p>Consider the first sample. If you do not hack any solutions, you will win the contest (scoreboard to the left). However, if you hack the solution of the first problem of the third participant (the only one you can hack), the maximum score for the first problem will change and you will finish second (scoreboard to the right). </p><center> <img class="tex-graphics" src="file://CQIsY6z4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
