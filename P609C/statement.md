## Description

<div><p>In the school computer room there are <span class="tex-span"><i>n</i></span> servers which are responsible for processing several computing tasks. You know the number of scheduled tasks for each server: there are <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> tasks assigned to the <span class="tex-span"><i>i</i></span>-th server.</p><p>In order to balance the load for each server, you want to reassign some tasks to make the difference between the most loaded server and the least loaded server as small as possible. In other words you want to minimize expression <span class="tex-span"><i>m</i><sub class="lower-index"><i>a</i></sub> - <i>m</i><sub class="lower-index"><i>b</i></sub></span>, where <span class="tex-span"><i>a</i></span> is the most loaded server and <span class="tex-span"><i>b</i></span> is the least loaded one.</p><p>In one second you can reassign a single task. Thus in one second you can choose any pair of servers and move a single task from one server to another.</p><p>Write a program to find the minimum number of seconds needed to balance the load of servers.</p></div><div class="input-specification"><p>The first line contains positive number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the servers. </p><p>The second line contains the sequence of non-negative integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> is the number of tasks assigned to the <span class="tex-span"><i>i</i></span>-th server.</p></div><div class="output-specification"><p>Print the minimum number of seconds required to balance the load.</p></div>

## Input

<p>The first line contains positive number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the servers. </p><p>The second line contains the sequence of non-negative integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> is the number of tasks assigned to the <span class="tex-span"><i>i</i></span>-th server.</p>

## Output

<p>Print the minimum number of seconds required to balance the load.</p>





```input1
2
1 6

```




```input2
7
10 11 10 11 10 11 11

```




```input3
5
1 2 3 4 5

```




```output1
2

```




```output2
0

```




```output3
3

```



## Note

<p>In the first example two seconds are needed. In each second, a single task from server #2 should be moved to server #1. After two seconds there should be 3 tasks on server #1 and 4 tasks on server #2.</p><p>In the second example the load is already balanced.</p><p>A possible sequence of task movements for the third example is:</p><ol> <li> move a task from server #4 to server #1 (the sequence <span class="tex-span"><i>m</i></span> becomes: 2 2 3 3 5); </li><li> then move task from server #5 to server #1 (the sequence <span class="tex-span"><i>m</i></span> becomes: 3 2 3 3 4); </li><li> then move task from server #5 to server #2 (the sequence <span class="tex-span"><i>m</i></span> becomes: 3 3 3 3 3). </li></ol><p>The above sequence is one of several possible ways to balance the load of servers in three seconds.</p>
