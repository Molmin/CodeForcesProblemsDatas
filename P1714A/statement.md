## Description

<div><p>Vlad, like everyone else, loves to sleep very much.</p><p>Every day Vlad has to do $n$ things, each at a certain time. For each of these things, he has an alarm clock set, the $i$-th of them is triggered on $h_i$ hours $m_i$ minutes every day ($0 \le h_i &lt; 24, 0 \le m_i &lt; 60$). Vlad uses the $24$-hour time format, so after $h=12, m=59$ comes $h=13, m=0$ and after $h=23, m=59$ comes $h=0, m=0$.</p><p>This time Vlad went to bed at $H$ hours $M$ minutes ($0 \le H &lt; 24, 0 \le M &lt; 60$) and asks you to answer: how much he will be able to sleep until the next alarm clock.</p><p>If any alarm clock rings at the time when he went to bed, then he will sleep for a period of time of length $0$.</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 100$) — the number of test cases in the test.</p><p>The first line of the case contains three integers $n$, $H$ and $M$ ($1 \le n \le 10, 0 \le H &lt; 24, 0 \le M &lt; 60$) — the number of alarms and the time Vlad went to bed.</p><p>The following $n$ lines contain two numbers each $h_i$ and $m_i$ ($0 \le h_i &lt; 24, 0 \le m_i &lt; 60$) — the time of the $i$ alarm. It is acceptable that two or more alarms will trigger at the same time.</p><p>Numbers describing time do not contain leading zeros.</p></div><div class="output-specification"><p>Output $t$ lines, each containing the answer to the corresponding test case. As an answer, output two numbers &nbsp;— the number of hours and minutes that Vlad will sleep, respectively. If any alarm clock rings at the time when he went to bed, the answer will be <span class="tex-font-style-tt">0 0</span>.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 100$) — the number of test cases in the test.</p><p>The first line of the case contains three integers $n$, $H$ and $M$ ($1 \le n \le 10, 0 \le H &lt; 24, 0 \le M &lt; 60$) — the number of alarms and the time Vlad went to bed.</p><p>The following $n$ lines contain two numbers each $h_i$ and $m_i$ ($0 \le h_i &lt; 24, 0 \le m_i &lt; 60$) — the time of the $i$ alarm. It is acceptable that two or more alarms will trigger at the same time.</p><p>Numbers describing time do not contain leading zeros.</p>

## Output

<p>Output $t$ lines, each containing the answer to the corresponding test case. As an answer, output two numbers &nbsp;— the number of hours and minutes that Vlad will sleep, respectively. If any alarm clock rings at the time when he went to bed, the answer will be <span class="tex-font-style-tt">0 0</span>.</p>





```input1|2,3,8,9,10
3
1 6 13
8 0
3 6 0
12 30
14 45
6 0
2 23 35
20 15
10 30
```




```output1
1 47
0 0
10 55
```


