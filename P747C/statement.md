## Description

<div><p>There are <span class="tex-span"><i>n</i></span> servers in a laboratory, each of them can perform tasks. Each server has a unique id&nbsp;— integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>It is known that during the day <span class="tex-span"><i>q</i></span> tasks will come, the <span class="tex-span"><i>i</i></span>-th of them is characterized with three integers: <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the moment in seconds in which the task will come, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the number of servers needed to perform it, and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the time needed to perform this task in seconds. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>To perform the <span class="tex-span"><i>i</i></span>-th task you need <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> servers which are unoccupied in the second <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. After the servers begin to perform the task, each of them will be busy over the next <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> seconds. Thus, they will be busy in seconds <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> + 1, ..., <i>t</i><sub class="lower-index"><i>i</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub> - 1</span>. For performing the task, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> servers with the smallest ids will be chosen from all the unoccupied servers. If in the second <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> there are not enough unoccupied servers, the task is ignored.</p><p>Write the program that determines which tasks will be performed and which will be ignored.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of servers and the number of tasks. </p><p>Next <span class="tex-span"><i>q</i></span> lines contains three integers each, the <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the moment in seconds in which the <span class="tex-span"><i>i</i></span>-th task will come, the number of servers needed to perform it, and the time needed to perform this task in seconds. The tasks are given in a chronological order and they will come in distinct seconds. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. If the <span class="tex-span"><i>i</i></span>-th task will be performed by the servers, print in the <span class="tex-span"><i>i</i></span>-th line the sum of servers' ids on which this task will be performed. Otherwise, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of servers and the number of tasks. </p><p>Next <span class="tex-span"><i>q</i></span> lines contains three integers each, the <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the moment in seconds in which the <span class="tex-span"><i>i</i></span>-th task will come, the number of servers needed to perform it, and the time needed to perform this task in seconds. The tasks are given in a chronological order and they will come in distinct seconds. </p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. If the <span class="tex-span"><i>i</i></span>-th task will be performed by the servers, print in the <span class="tex-span"><i>i</i></span>-th line the sum of servers' ids on which this task will be performed. Otherwise, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 3
1 3 2
2 2 1
3 4 3

```




```input2
3 2
3 2 3
5 1 2

```




```input3
8 6
1 3 20
4 2 1
6 5 5
10 1 1
15 3 6
21 8 8

```




```output1
6
-1
10

```




```output2
3
3

```




```output3
6
9
30
-1
15
36

```



## Note

<p>In the first example in the second <span class="tex-span">1</span> the first task will come, it will be performed on the servers with ids <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span> (the sum of the ids equals <span class="tex-span">6</span>) during two seconds. In the second <span class="tex-span">2</span> the second task will come, it will be ignored, because only the server <span class="tex-span">4</span> will be unoccupied at that second. In the second <span class="tex-span">3</span> the third task will come. By this time, servers with the ids <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span> will be unoccupied again, so the third task will be done on all the servers with the ids <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span> (the sum of the ids is <span class="tex-span">10</span>).</p><p>In the second example in the second <span class="tex-span">3</span> the first task will come, it will be performed on the servers with ids <span class="tex-span">1</span> and <span class="tex-span">2</span> (the sum of the ids is <span class="tex-span">3</span>) during three seconds. In the second <span class="tex-span">5</span> the second task will come, it will be performed on the server <span class="tex-span">3</span>, because the first two servers will be busy performing the first task.</p>
