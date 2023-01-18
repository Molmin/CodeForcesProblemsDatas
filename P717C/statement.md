## Description

<div><p>Harry Water, Ronaldo, Her-my-oh-knee and their friends have started a new school year at their MDCS School of Speechcraft and Misery. At the time, they are very happy to have seen each other after a long time. The sun is shining, birds are singing, flowers are blooming, and their Potions class teacher, professor Snipe is sulky as usual. Due to his angst fueled by disappointment in his own life, he has given them a lot of homework in Potions class. </p><p>Each of the <span class="tex-span"><i>n</i></span> students has been assigned a single task. Some students do certain tasks faster than others. Thus, they want to redistribute the tasks so that each student still does exactly one task, and that all tasks are finished. Each student has their own laziness level, and each task has its own difficulty level. Professor Snipe is trying hard to improve their work ethics, so each student’s laziness level is equal to their task’s difficulty level. Both sets of values are given by the sequence <span class="tex-span"><i>a</i></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents both the laziness level of the <span class="tex-span"><i>i</i></span>-th student and the difficulty of his task. </p><p>The time a student needs to finish a task is equal to the product of their laziness level and the task’s difficulty. They are wondering, what is the minimum possible total time they must spend to finish all tasks if they distribute them in the optimal way. Each person should receive one task and each task should be given to one person. Print the answer modulo <span class="tex-span">10 007</span>.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of tasks. The next <span class="tex-span"><i>n</i></span> lines contain exactly one integer number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— both the difficulty of the initial task and the laziness of the <span class="tex-span"><i>i</i></span>-th students.</p></div><div class="output-specification"><p>Print the minimum total time to finish all tasks modulo <span class="tex-span">10 007</span>.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of tasks. The next <span class="tex-span"><i>n</i></span> lines contain exactly one integer number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>)&nbsp;— both the difficulty of the initial task and the laziness of the <span class="tex-span"><i>i</i></span>-th students.</p>

## Output

<p>Print the minimum total time to finish all tasks modulo <span class="tex-span">10 007</span>.</p>





```input1
2
1
3

```




```output1
6

```



## Note

<p>In the first sample, if the students switch their tasks, they will be able to finish them in <span class="tex-span">3 + 3 = 6</span> time units.</p>
