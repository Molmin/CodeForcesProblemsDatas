## Description

<div><p>Eonathan Eostar decided to learn the magic of multiprocessor systems. He has a full binary tree of tasks with height $h$. In the beginning, there is only one <span class="tex-font-style-underline">ready</span> task in the tree&nbsp;— the task in the root. At each moment of time, $p$ processes choose at most $p$ <span class="tex-font-style-underline">ready</span> tasks and perform them. After that, tasks whose parents were performed become <span class="tex-font-style-underline">ready</span> for the next moment of time. Once the task becomes <span class="tex-font-style-underline">ready</span>, it stays <span class="tex-font-style-underline">ready</span> until it is performed. </p><p>You shall calculate the smallest number of time moments the system needs to perform all the tasks.</p></div><div class="input-specification"><p>The first line of the input contains the number of tests $t$ ($1 \leq t \leq 5\cdot 10^5$). Each of the next $t$ lines contains the description of a test. A test is described by two integers $h$ ($1 \leq h \leq 50$) and $p$ ($1 \leq p \leq 10^4$)&nbsp;— the height of the full binary tree and the number of processes. It is guaranteed that all the tests are different.</p></div><div class="output-specification"><p>For each test output one integer on a separate line&nbsp;— the smallest number of time moments the system needs to perform all the tasks.</p></div>

## Input

<p>The first line of the input contains the number of tests $t$ ($1 \leq t \leq 5\cdot 10^5$). Each of the next $t$ lines contains the description of a test. A test is described by two integers $h$ ($1 \leq h \leq 50$) and $p$ ($1 \leq p \leq 10^4$)&nbsp;— the height of the full binary tree and the number of processes. It is guaranteed that all the tests are different.</p>

## Output

<p>For each test output one integer on a separate line&nbsp;— the smallest number of time moments the system needs to perform all the tasks.</p>





```input1
3
3 1
3 2
10 6
```




```output1
7
4
173
```



## Note

<p>Let us consider the second test from the sample input. There is a full binary tree of height $3$ and there are two processes. At the first moment of time, there is only one ready task, $1$, and $p_1$ performs it. At the second moment of time, there are two ready tasks, $2$ and $3$, and the processes perform them. At the third moment of time, there are four ready tasks, $4$, $5$, $6$, and $7$, and $p_1$ performs $6$ and $p_2$ performs $5$. At the fourth moment of time, there are two ready tasks, $4$ and $7$, and the processes perform them. Thus, the system spends $4$ moments of time to perform all the tasks.</p><p><img class="tex-graphics" src="file://nZprIGK4.png" style="max-width: 100.0%;max-height: 100.0%;" width="680px"></p>
