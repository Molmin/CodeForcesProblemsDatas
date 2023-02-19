## Description

<div><p>Recently, Polycarp completed $n$ successive tasks.</p><p>For each completed task, the time $s_i$ is known when it was given, no two tasks were given at the same time. Also given is the time $f_i$ when the task was completed. For each task, there is an unknown value $d_i$ ($d_i&gt;0$)&nbsp;— <span class="tex-font-style-bf">duration of task execution</span>.</p><p>It is known that the tasks were completed in the order in which they came. Polycarp performed the tasks as follows:</p><ul> <li> As soon as the very first task came, Polycarp immediately began to carry it out. </li><li> If a new task arrived before Polycarp finished the previous one, he put the new task at the end of the queue. </li><li> When Polycarp finished executing the next task and the queue was not empty, he <span class="tex-font-style-bf">immediately</span> took a new task from the head of the queue (if the queue is empty — he just waited for the next task). </li></ul><p>Find $d_i$ (duration) of each task.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The descriptions of the input data sets follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains exactly $n$ integers $s_1 &lt; s_2 &lt; \dots &lt; s_n$ ($0 \le s_i \le 10^9$).</p><p>The third line of each test case contains exactly $n$ integers $f_1 &lt; f_2 &lt; \dots &lt; f_n$ ($s_i &lt; f_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each of $t$ test cases print $n$ positive integers $d_1, d_2, \dots, d_n$&nbsp;— the duration of each task.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The descriptions of the input data sets follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$).</p><p>The second line of each test case contains exactly $n$ integers $s_1 &lt; s_2 &lt; \dots &lt; s_n$ ($0 \le s_i \le 10^9$).</p><p>The third line of each test case contains exactly $n$ integers $f_1 &lt; f_2 &lt; \dots &lt; f_n$ ($s_i &lt; f_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each of $t$ test cases print $n$ positive integers $d_1, d_2, \dots, d_n$&nbsp;— the duration of each task.</p>





```input1
4
3
0 3 7
2 10 11
2
10 15
11 16
9
12 16 90 195 1456 1569 3001 5237 19275
13 199 200 260 9100 10000 10914 91066 5735533
1
0
1000000000
```




```output1
2 7 1 
1 1 
1 183 1 60 7644 900 914 80152 5644467 
1000000000
```



## Note

<p>First test case:</p><p>The queue is empty at the beginning: $[ ]$. And that's where the first task comes in. At time $2$, Polycarp finishes doing the first task, so the duration of the first task is $2$. The queue is empty so Polycarp is just waiting.</p><p>At time $3$, the second task arrives. And at time $7$, the third task arrives, and now the queue looks like this: $[7]$.</p><p>At the time $10$, Polycarp finishes doing the second task, as a result, the duration of the second task is $7$.</p><p>And at time $10$, Polycarp immediately starts doing the third task and finishes at time $11$. As a result, the duration of the third task is $1$.</p><center> <img class="tex-graphics" src="file://RvBqsWsX.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">An example of the first test case.</span> </center>
