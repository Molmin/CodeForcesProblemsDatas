## Description

<div><p>Let's consider a network printer that functions like that. It starts working at time 0. In each second it can print one page of a text. At some moments of time the printer receives printing tasks. We know that a printer received <span class="tex-span"><i>n</i></span> tasks. Let's number the tasks by consecutive integers from 1 to <span class="tex-span"><i>n</i></span>. Then the task number <span class="tex-span"><i>i</i></span> is characterised by three integers: <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the time when the task came, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is the task's volume (in pages) and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the task's priority. The priorities of all tasks are distinct.</p><p>When the printer receives a task, the task goes to the queue and remains there until all pages from this task are printed. The printer chooses a page to print each time when it either stops printing some page or when it is free and receives a new task. Among all tasks that are in the queue at this moment, the printer chooses the task with the highest priority and next second prints an unprinted page from this task. You can assume that a task goes to the queue immediately, that's why if a task has just arrived by time <span class="tex-span"><i>t</i></span>, the printer can already choose it for printing.</p><p>You are given full information about all tasks except for one: you don't know this task's priority. However, we know the time when the last page from this task was finished printing. Given this information, find the unknown priority value and determine the moments of time when the printer finished printing each task.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>). Next <span class="tex-span"><i>n</i></span> lines describe the tasks. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Exactly one task (let's assume that his number is <span class="tex-span"><i>x</i></span>) has number <span class="tex-font-style-tt">-1</span> written instead of the priority. All priorities are different. The last line contains integer <span class="tex-span"><i>T</i></span> — the time when the printer finished printing the last page of task <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">15</sup></span>). Numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily distinct. The tasks in the input are written in the arbitrary order.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span> — the priority of the task number <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>x</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, remember that all priorities should be distinct). Then print <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them represents the moment of time when the last page of the task number <span class="tex-span"><i>i</i></span> finished printing. </p><p>It is guaranteed that at least one solution exists. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50000</span>). Next <span class="tex-span"><i>n</i></span> lines describe the tasks. The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, separated by single spaces (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Exactly one task (let's assume that his number is <span class="tex-span"><i>x</i></span>) has number <span class="tex-font-style-tt">-1</span> written instead of the priority. All priorities are different. The last line contains integer <span class="tex-span"><i>T</i></span> — the time when the printer finished printing the last page of task <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 10<sup class="upper-index">15</sup></span>). Numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are not necessarily distinct. The tasks in the input are written in the arbitrary order.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>x</i></sub></span> — the priority of the task number <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>x</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, remember that all priorities should be distinct). Then print <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them represents the moment of time when the last page of the task number <span class="tex-span"><i>i</i></span> finished printing. </p><p>It is guaranteed that at least one solution exists. If there are multiple solutions, print any of them.</p>





```input1
3
4 3 -1
0 2 2
1 3 3
7

```




```input2
3
3 1 2
2 3 3
3 1 -1
4

```




```output1
4
7 8 4

```




```output2
4
7 6 4

```



## Note

<p>Let's consider the first test case. Let's assume that the unknown priority equals 4, then the printer's actions for each second are as follows:</p><ul> <li> the beginning of the 1-st second (time 0). The queue has task 2. The printer prints the first page of this task; </li><li> the beginning of the 2-nd second (time 1). The queue has tasks 2 and 3. The printer prints the first page of task 3; </li><li> the beginning of the 3-rd second (time 2). The queue has tasks 2 and 3. The printer prints the second page of task 3; </li><li> the beginning of the 4-th second (time 3). The queue has tasks 2 and 3. The printer prints the third (last) page of task 3. Thus, by the end of the 4-th second this task will have been printed; </li><li> the beginning of the 5-th second (time 4). The queue has tasks 2 and 1. The printer prints the first page of task 1; </li><li> the beginning of the 6-th second (time 5). The queue has tasks 2 and 1. The printer prints the second page of task 1; </li><li> the beginning of the 7-th second (time 6). The queue has tasks 2 and 1. The printer prints the third (last) page of task 1. Thus, by the end of the 7-th second this task will have been printed; </li><li> the beginning of the 8-th second (time 7). The queue has task 2. The printer prints the second (last) page of task 2. Thus, by the end of the 8-th second this task will have been printed. </li></ul><p>In the end, task number 1 will have been printed by the end of the 7-th second, as was required. And tasks 2 and 3 are printed by the end of the of the 8-th and the 4-th second correspondingly.</p>
