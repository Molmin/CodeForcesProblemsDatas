## Description

<div><p>You are given a program you want to execute as a set of tasks organized in a dependency graph. The dependency graph is a directed acyclic graph: each task can depend on results of one or several other tasks, and there are no directed circular dependencies between tasks. A task can only be executed if all tasks it depends on have already completed.</p><p>Some of the tasks in the graph can only be executed on a coprocessor, and the rest can only be executed on the main processor. In one coprocessor call you can send it a set of tasks which can only be executed on it. For each task of the set, all tasks on which it depends must be either already completed or be included in the set. The main processor starts the program execution and gets the results of tasks executed on the coprocessor automatically.</p><p>Find the minimal number of coprocessor calls which are necessary to execute the given program.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>) — the total number of tasks given, and <span class="tex-span"><i>M</i></span> (<span class="tex-span">0 ≤ <i>M</i> ≤ 10<sup class="upper-index">5</sup></span>) — the total number of dependencies between tasks.</p><p>The next line contains <span class="tex-span"><i>N</i></span> space-separated integers <img align="middle" class="tex-formula" src="file://nVL1OO55.png" style="max-width: 100.0%;max-height: 100.0%;">. If <span class="tex-span"><i>E</i><sub class="lower-index"><i>i</i></sub> = 0</span>, task <span class="tex-span"><i>i</i></span> can only be executed on the main processor, otherwise it can only be executed on the coprocessor.</p><p>The next <span class="tex-span"><i>M</i></span> lines describe the dependencies between tasks. Each line contains two space-separated integers <span class="tex-span"><i>T</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> and means that task <span class="tex-span"><i>T</i><sub class="lower-index">1</sub></span> depends on task <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>T</i><sub class="lower-index">1</sub> ≠ <i>T</i><sub class="lower-index">2</sub></span>). Tasks are indexed from <span class="tex-span">0</span> to <span class="tex-span"><i>N</i> - 1</span>. All <span class="tex-span"><i>M</i></span> pairs <span class="tex-span">(<i>T</i><sub class="lower-index">1</sub>, <i>T</i><sub class="lower-index">2</sub>)</span> are distinct. It is guaranteed that there are no circular dependencies between tasks.</p></div><div class="output-specification"><p>Output one line containing an integer — the minimal number of coprocessor calls necessary to execute the program.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>) — the total number of tasks given, and <span class="tex-span"><i>M</i></span> (<span class="tex-span">0 ≤ <i>M</i> ≤ 10<sup class="upper-index">5</sup></span>) — the total number of dependencies between tasks.</p><p>The next line contains <span class="tex-span"><i>N</i></span> space-separated integers <img align="middle" class="tex-formula" src="file://nVL1OO55.png" style="max-width: 100.0%;max-height: 100.0%;">. If <span class="tex-span"><i>E</i><sub class="lower-index"><i>i</i></sub> = 0</span>, task <span class="tex-span"><i>i</i></span> can only be executed on the main processor, otherwise it can only be executed on the coprocessor.</p><p>The next <span class="tex-span"><i>M</i></span> lines describe the dependencies between tasks. Each line contains two space-separated integers <span class="tex-span"><i>T</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> and means that task <span class="tex-span"><i>T</i><sub class="lower-index">1</sub></span> depends on task <span class="tex-span"><i>T</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>T</i><sub class="lower-index">1</sub> ≠ <i>T</i><sub class="lower-index">2</sub></span>). Tasks are indexed from <span class="tex-span">0</span> to <span class="tex-span"><i>N</i> - 1</span>. All <span class="tex-span"><i>M</i></span> pairs <span class="tex-span">(<i>T</i><sub class="lower-index">1</sub>, <i>T</i><sub class="lower-index">2</sub>)</span> are distinct. It is guaranteed that there are no circular dependencies between tasks.</p>

## Output

<p>Output one line containing an integer — the minimal number of coprocessor calls necessary to execute the program.</p>





```input1
4 3
0 1 0 1
0 1
1 2
2 3

```




```input2
4 3
1 1 1 0
0 1
0 2
3 0

```




```output1
2

```




```output2
1

```



## Note

<p>In the first test, tasks 1 and 3 can only be executed on the coprocessor. The dependency graph is linear, so the tasks must be executed in order 3 -&gt; 2 -&gt; 1 -&gt; 0. You have to call coprocessor twice: first you call it for task 3, then you execute task 2 on the main processor, then you call it for for task 1, and finally you execute task 0 on the main processor.</p><p>In the second test, tasks 0, 1 and 2 can only be executed on the coprocessor. Tasks 1 and 2 have no dependencies, and task 0 depends on tasks 1 and 2, so all three tasks 0, 1 and 2 can be sent in one coprocessor call. After that task 3 is executed on the main processor.</p>
