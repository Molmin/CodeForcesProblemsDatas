## Description

<div><p>Polycarp takes part in a math show. He is given <span class="tex-span"><i>n</i></span> tasks, each consists of <span class="tex-span"><i>k</i></span> subtasks, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>k</i></span>. It takes him <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> minutes to solve the <span class="tex-span"><i>j</i></span>-th subtask of any task. Thus, time required to solve a subtask depends only on its index, but not on the task itself. Polycarp can solve subtasks in any order.</p><p>By solving subtask of arbitrary problem he earns one point. Thus, the number of points for task is equal to the number of solved subtasks in it. Moreover, if Polycarp <span class="tex-font-style-it">completely</span> solves the task (solves all <span class="tex-span"><i>k</i></span> of its subtasks), he recieves one extra point. Thus, total number of points he recieves for the complete solution of the task is <span class="tex-span"><i>k</i> + 1</span>.</p><p>Polycarp has <span class="tex-span"><i>M</i></span> minutes of time. What is the maximum number of points he can earn?</p></div><div class="input-specification"><p>The first line contains three integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 45</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 45</span>, <span class="tex-span">0 ≤ <i>M</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>k</i></span> integer numbers, values <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 1000000</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> is the time in minutes required to solve <span class="tex-span"><i>j</i></span>-th subtask of any task.</p></div><div class="output-specification"><p>Print the maximum amount of points Polycarp can earn in <span class="tex-span"><i>M</i></span> minutes.</p></div>

## Input

<p>The first line contains three integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 45</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 45</span>, <span class="tex-span">0 ≤ <i>M</i> ≤ 2·10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>k</i></span> integer numbers, values <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 1000000</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> is the time in minutes required to solve <span class="tex-span"><i>j</i></span>-th subtask of any task.</p>

## Output

<p>Print the maximum amount of points Polycarp can earn in <span class="tex-span"><i>M</i></span> minutes.</p>





```input1
3 4 11
1 2 3 4

```




```input2
5 5 10
1 2 4 8 16

```




```output1
6

```




```output2
7

```



## Note

<p>In the first example Polycarp can complete the first task and spend <span class="tex-span">1 + 2 + 3 + 4 = 10</span> minutes. He also has the time to solve one subtask of the second task in one minute.</p><p>In the second example Polycarp can solve the first subtask of all five tasks and spend <span class="tex-span">5·1 = 5</span> minutes. Also he can solve the second subtasks of two tasks and spend <span class="tex-span">2·2 = 4</span> minutes. Thus, he earns <span class="tex-span">5 + 2 = 7</span> points in total.</p>
