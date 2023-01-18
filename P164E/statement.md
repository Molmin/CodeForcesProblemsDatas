## Description

<div><p>Polycarpus has many tasks. Each task is characterized by three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Three integers <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>)</span> mean that to perform task <span class="tex-span"><i>i</i></span>, one needs to choose an integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>;&nbsp;<i>s</i><sub class="lower-index"><i>i</i></sub> + <i>t</i><sub class="lower-index"><i>i</i></sub> - 1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub>)</span>, then the task will be carried out continuously for <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> units of time, starting at time <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and up to time <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> + <i>t</i><sub class="lower-index"><i>i</i></sub> - 1</span>, inclusive. In other words, a task is performed for a continuous period of time lasting <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, should be started no earlier than <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, and completed no later than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Polycarpus's tasks have a surprising property: for any task <span class="tex-span"><i>j</i>, <i>k</i></span> (with <span class="tex-span"><i>j</i> &lt; <i>k</i></span>) <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> &lt; <i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub> &lt; <i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>Let's suppose there is an ordered set of tasks <span class="tex-span"><i>A</i></span>, containing <span class="tex-span">|<i>A</i>|</span> tasks. We'll assume that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = (<i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>, <i>t</i><sub class="lower-index"><i>j</i></sub>)</span> <span class="tex-span">(1 ≤ <i>j</i> ≤ |<i>A</i>|)</span>. Also, we'll assume that the tasks are ordered by increasing <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> with the increase in number.</p><p>Let's consider the following recursive function <span class="tex-span"><i>f</i></span>, whose argument is an ordered set of tasks <span class="tex-span"><i>A</i></span>, and the result is an integer. The function <span class="tex-span"><i>f</i>(<i>A</i>)</span> is defined by the greedy algorithm, which is described below in a pseudo-language of programming.</p><ul> <li> Step 1. <img align="middle" class="tex-formula" src="file://V2XuFdNt.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span"><i>ans</i> = 0</span>. </li><li> Step 2. We consider all tasks in the order of increasing of their numbers in the set <span class="tex-span"><i>A</i></span>. Lets define the current task counter <span class="tex-span"><i>i</i> = 0</span>. </li><li> Step 3. Consider the next task: <span class="tex-span"><i>i</i> = <i>i</i> + 1</span>. If <span class="tex-span"><i>i</i> &gt; |<i>A</i>|</span> fulfilled, then go to the 8 step. </li><li> Step 4. If you can get the task done starting at time <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = max<span class="tex-span">(<i>ans</i> + 1, <i>l</i><sub class="lower-index"><i>i</i></sub>)</span>, then do the task <span class="tex-span"><i>i</i></span>: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = max(<span class="tex-span"><i>ans</i> + 1</span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>), <span class="tex-span"><i>ans</i> = <i>s</i><sub class="lower-index"><i>i</i></sub> + <i>t</i><sub class="lower-index"><i>i</i></sub> - 1</span>, <img align="middle" class="tex-formula" src="file://vC9QLyjS.png" style="max-width: 100.0%;max-height: 100.0%;">. Go to the next task (step 3). </li><li> Step 5. Otherwise, find such task <img align="middle" class="tex-formula" src="file://U1Vpumdi.png" style="max-width: 100.0%;max-height: 100.0%;">, that first, task <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> can be done at time <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = max<img align="middle" class="tex-formula" src="file://faN64M4G.png" style="max-width: 100.0%;max-height: 100.0%;">, and secondly, the value of <img align="middle" class="tex-formula" src="file://bXG59Amn.png" style="max-width: 100.0%;max-height: 100.0%;"> is positive and takes the maximum value among all <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> that satisfy the first condition. If you can choose multiple tasks as <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>, choose the one with the maximum number in set <span class="tex-span"><i>A</i></span>. </li><li> Step 6. If you managed to choose task <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>, then <img align="middle" class="tex-formula" src="file://jncMvQvp.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://WJfYpVAA.png" style="max-width: 100.0%;max-height: 100.0%;">. Go to the next task (step 3). </li><li> Step 7. If you didn't manage to choose task <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span>, then skip task <span class="tex-span"><i>i</i></span>. Go to the next task (step 3). </li><li> Step 8. Return <span class="tex-span"><i>ans</i></span> as a result of executing <span class="tex-span"><i>f</i>(<i>A</i>)</span>. </li></ul><p>Polycarpus got entangled in all these formulas and definitions, so he asked you to simulate the execution of the function <span class="tex-span"><i>f</i></span>, calculate the value of <span class="tex-span"><i>f</i>(<i>A</i>)</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tasks in set <span class="tex-span"><i>A</i></span>. </p><p>Then <span class="tex-span"><i>n</i></span> lines describe the tasks. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> - <i>l</i><sub class="lower-index"><i>i</i></sub> + 1</span>) — the description of the <span class="tex-span"><i>i</i></span>-th task.</p><p>It is guaranteed that for any tasks <span class="tex-span"><i>j</i>, <i>k</i></span> (considering that <span class="tex-span"><i>j</i> &lt; <i>k</i></span>) the following is true: <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> &lt; <i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub> &lt; <i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p></div><div class="output-specification"><p>For each task <span class="tex-span"><i>i</i></span> print a single integer — the result of processing task <span class="tex-span"><i>i</i></span> on the <span class="tex-span"><i>i</i></span>-th iteration of the cycle (step 3) in function <span class="tex-span"><i>f</i>(<i>A</i>)</span>. In the <span class="tex-span"><i>i</i></span>-th line print:</p><ul> <li> 0 — if you managed to add task <span class="tex-span"><i>i</i></span> on step 4. </li><li> -1 — if you didn't manage to add or replace task <span class="tex-span"><i>i</i></span> (step 7). </li><li> <span class="tex-span"><i>res</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>res</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — if you managed to replace the task (step 6): <span class="tex-span"><i>res</i><sub class="lower-index"><i>i</i></sub></span> equals the task number (in set <span class="tex-span"><i>A</i></span>), that should be chosen as <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> and replaced by task <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tasks in set <span class="tex-span"><i>A</i></span>. </p><p>Then <span class="tex-span"><i>n</i></span> lines describe the tasks. The <span class="tex-span"><i>i</i></span>-th line contains three space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> - <i>l</i><sub class="lower-index"><i>i</i></sub> + 1</span>) — the description of the <span class="tex-span"><i>i</i></span>-th task.</p><p>It is guaranteed that for any tasks <span class="tex-span"><i>j</i>, <i>k</i></span> (considering that <span class="tex-span"><i>j</i> &lt; <i>k</i></span>) the following is true: <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> &lt; <i>l</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub> &lt; <i>r</i><sub class="lower-index"><i>k</i></sub></span>.</p>

## Output

<p>For each task <span class="tex-span"><i>i</i></span> print a single integer — the result of processing task <span class="tex-span"><i>i</i></span> on the <span class="tex-span"><i>i</i></span>-th iteration of the cycle (step 3) in function <span class="tex-span"><i>f</i>(<i>A</i>)</span>. In the <span class="tex-span"><i>i</i></span>-th line print:</p><ul> <li> 0 — if you managed to add task <span class="tex-span"><i>i</i></span> on step 4. </li><li> -1 — if you didn't manage to add or replace task <span class="tex-span"><i>i</i></span> (step 7). </li><li> <span class="tex-span"><i>res</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>res</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — if you managed to replace the task (step 6): <span class="tex-span"><i>res</i><sub class="lower-index"><i>i</i></sub></span> equals the task number (in set <span class="tex-span"><i>A</i></span>), that should be chosen as <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub></span> and replaced by task <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul>





```input1
5
1 8 5
2 9 3
3 10 3
8 11 4
11 12 2

```




```input2
13
1 8 5
2 9 4
3 10 1
4 11 3
8 12 5
9 13 5
10 14 5
11 15 1
12 16 1
13 17 1
14 18 3
15 19 3
16 20 2

```




```output1
0 0 1 0 -1
```




```output2
0 0 0 2 -1 -1 0 0 0 0 7 0 12
```


