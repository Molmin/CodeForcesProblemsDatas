## Description

<div><p>Monocarp is planning to host a martial arts tournament. There will be three divisions based on weight: lightweight, middleweight and heavyweight. The winner of each division will be determined by a single elimination system.</p><p>In particular, that implies that the number of participants in each division should be a power of two. Additionally, each division should have a non-zero amount of participants.</p><p>$n$ participants have registered for the tournament so far, the $i$-th of them weighs $a_i$. To split participants into divisions, Monocarp is going to establish two integer weight boundaries $x$ and $y$ ($x &lt; y$). </p><p>All participants who weigh strictly less than $x$ will be considered lightweight. All participants who weigh greater or equal to $y$ will be considered heavyweight. The remaining participants will be considered middleweight.</p><p>It's possible that the distribution doesn't make the number of participants in each division a power of two. It can also lead to empty divisions. To fix the issues, Monocarp can invite an arbitrary number of participants to each division.</p><p>Note that Monocarp can't kick out any of the $n$ participants who have already registered for the tournament.</p><p>However, he wants to invite as little extra participants as possible. Help Monocarp to choose $x$ and $y$ in such a way that the total amount of extra participants required is as small as possible. Output that amount.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of the registered participants.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the weights of the registered participants.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the smallest number of extra participants Monocarp is required to invite after he chooses the weight boundaries $x$ and $y$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of the registered participants.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the weights of the registered participants.</p><p>The sum of $n$ over all testcases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the smallest number of extra participants Monocarp is required to invite after he chooses the weight boundaries $x$ and $y$.</p>





```input1
4
4
3 1 2 1
1
1
6
2 2 2 1 1 1
8
6 3 6 3 6 3 6 6
```




```output1
0
2
3
2
```



## Note

<p>In the first testcase of the example, Monocarp can choose $x=2$ and $y=3$. Lightweight, middleweight and heavyweight divisions will have $2$, $1$ and $1$ participants, respectively. They all are powers of two, so no extra participants are required.</p><p>In the second testcase of the example, regardless of the choice of $x$ and $y$, one division will have $1$ participant, the rest will have $0$. Thus, Monocarp will have to invite $1$ participant into both of the remaining divisions.</p><p>In the third testcase of the example, Monocarp can choose $x=1$ and $y=2$. Lightweight, middleweight and heavyweight divisions will have $0$, $3$ and $3$ participants, respectively. So an extra participant is needed in each division.</p><p>In the fourth testcase of the example, Monocarp can choose $x=8$ and $y=9$. Lightweight, middleweight and heavyweight divisions will have $8$, $0$ and $0$ participants, respectively. Middleweight and heavyweight division need an extra participant each.</p>
