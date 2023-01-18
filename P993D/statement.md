## Description

<div><p>You need to execute several tasks, each associated with number of processors it needs, and the compute power it will consume.</p><p>You have sufficient number of analog computers, each with enough processors for any task. Each computer can execute up to one task at a time, and no more than two tasks total. The first task can be any, the second task on each computer must use strictly less power than the first. You will assign between 1 and 2 tasks to each computer. You will then first execute the first task on each computer, wait for all of them to complete, and then execute the second task on each computer that has two tasks assigned.</p><p>If the average compute power per utilized processor (the sum of all consumed powers for all tasks presently running divided by the number of utilized processors) across all computers exceeds some unknown threshold during the execution of the first tasks, the entire system will blow up. There is no restriction on the second tasks execution. Find the lowest threshold for which it is possible.</p><p>Due to the specifics of the task, you need to print the answer multiplied by 1000 and rounded up.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of tasks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the amount of power required for the <span class="tex-span"><i>i</i></span>-th task.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of processors that <span class="tex-span"><i>i</i></span>-th task will utilize.</p></div><div class="output-specification"><p>Print a single integer value — the lowest threshold for which it is possible to assign all tasks in such a way that the system will not blow up after the first round of computation, multiplied by 1000 and rounded up.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of tasks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the amount of power required for the <span class="tex-span"><i>i</i></span>-th task.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of processors that <span class="tex-span"><i>i</i></span>-th task will utilize.</p>

## Output

<p>Print a single integer value — the lowest threshold for which it is possible to assign all tasks in such a way that the system will not blow up after the first round of computation, multiplied by 1000 and rounded up.</p>





```input1
6
8 10 9 9 8 10
1 1 1 1 1 1

```




```input2
6
8 10 9 9 8 10
1 10 5 5 1 10

```




```output1
9000

```




```output2
1160

```



## Note

<p>In the first example the best strategy is to run each task on a separate computer, getting average compute per processor during the first round equal to 9.</p><p>In the second task it is best to run tasks with compute 10 and 9 on one computer, tasks with compute 10 and 8 on another, and tasks with compute 9 and 8 on the last, averaging (10 + 10 + 9) / (10 + 10 + 5) = 1.16 compute power per processor during the first round.</p>
