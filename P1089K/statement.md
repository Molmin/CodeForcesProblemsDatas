## Description

<div><p>King Kog got annoyed of the usual laxity of his knights&nbsp;— they can break into his hall without prior notice! Thus, the King decided to build a reception with a queue where each knight chooses in advance the time when he will come and how long the visit will take. The knights are served in the order of the recorded time, but each knight has to wait until the visits of all the knights before him are finished.</p><p>Princess Keabeanie wants to see her father. However, she does not want to interrupt the knights so she joins the queue. Unfortunately, the knights change their minds very often&nbsp;— they can join the queue or cancel their visits. Please help the princess to understand how long she will have to wait until she sees her father if she enters the queue at the specified moments of time given the records at the reception.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $q$ ($1 \leq q \leq 3 \cdot 10^5$)&nbsp;— the number of events. An event can be of three types: <span class="tex-font-style-underline">join</span>, <span class="tex-font-style-underline">cancel</span>, or <span class="tex-font-style-underline">query</span>.</p><ul> <li> Join "<span class="tex-font-style-tt">+ $t$ $d$</span>" ($1 \leq t, d \leq 10^6$)&nbsp;— a new knight joins the queue, where $t$ is the time when the knight will come and $d$ is the duration of the visit.</li><li> Cancel "<span class="tex-font-style-tt">- $i$</span>" ($1 \leq i \leq q$)&nbsp;— the knight cancels the visit, where $i$ is the number (counted starting from one) of the corresponding join event in the list of all events.</li><li> Query "<span class="tex-font-style-tt">? $t$</span>" ($1 \leq t \leq 10^6$)&nbsp;— Keabeanie asks how long she will wait if she comes at the time $t$. </li></ul><p>It is guaranteed that after each event there are no two knights with the same entrance time in the queue. Cancel events refer to the previous joins that were not cancelled yet.</p><p>Keabeanie can come at the same time as some knight, but Keabeanie is very polite and she will wait for the knight to pass.</p></div><div class="output-specification"><p>For each query write a separate line with the amount of time Keabeanie will have to wait.</p></div>

## Input

<p>The first line of the input contains a single integer $q$ ($1 \leq q \leq 3 \cdot 10^5$)&nbsp;— the number of events. An event can be of three types: <span class="tex-font-style-underline">join</span>, <span class="tex-font-style-underline">cancel</span>, or <span class="tex-font-style-underline">query</span>.</p><ul> <li> Join "<span class="tex-font-style-tt">+ $t$ $d$</span>" ($1 \leq t, d \leq 10^6$)&nbsp;— a new knight joins the queue, where $t$ is the time when the knight will come and $d$ is the duration of the visit.</li><li> Cancel "<span class="tex-font-style-tt">- $i$</span>" ($1 \leq i \leq q$)&nbsp;— the knight cancels the visit, where $i$ is the number (counted starting from one) of the corresponding join event in the list of all events.</li><li> Query "<span class="tex-font-style-tt">? $t$</span>" ($1 \leq t \leq 10^6$)&nbsp;— Keabeanie asks how long she will wait if she comes at the time $t$. </li></ul><p>It is guaranteed that after each event there are no two knights with the same entrance time in the queue. Cancel events refer to the previous joins that were not cancelled yet.</p><p>Keabeanie can come at the same time as some knight, but Keabeanie is very polite and she will wait for the knight to pass.</p>

## Output

<p>For each query write a separate line with the amount of time Keabeanie will have to wait.</p>





```input1
19
? 3
+ 2 2
? 3
? 4
+ 5 2
? 5
? 6
+ 1 2
? 2
? 3
? 4
? 5
? 6
? 7
? 9
- 8
? 2
? 3
? 6
```




```output1
0
1
0
2
1
3
2
1
2
1
0
0
2
1
1
```


