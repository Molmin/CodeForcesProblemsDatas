## Description

<div><p><span class="tex-font-style-it">El Psy Kongroo.</span></p><p>Omkar is watching <span class="tex-font-style-it">Steins;Gate</span>.</p><p>In <span class="tex-font-style-it">Steins;Gate</span>, Okabe Rintarou needs to complete $n$ tasks ($1 \leq n \leq 2 \cdot 10^5$). Unfortunately, he doesn't know when he needs to complete the tasks.</p><p>Initially, the time is $0$. Time travel will now happen according to the following rules:</p><ul><li><p>For each $k = 1, 2, \ldots, n$, Okabe will realize at time $b_k$ that he was supposed to complete the $k$-th task at time $a_k$ ($a_k &lt; b_k$). </p></li><li><p>When he realizes this, if $k$-th task was already completed at time $a_k$, Okabe keeps the usual flow of time. Otherwise, he time travels to time $a_k$ then immediately completes the task.</p></li><li><p>If Okabe time travels to time $a_k$, all tasks completed after this time will become incomplete again. That is, for every $j$, if $a_j&gt;a_k$, the $j$-th task will become incomplete, if it was complete (if it was incomplete, nothing will change).</p></li><li><p>Okabe has bad memory, so he can time travel to time $a_k$ <span class="tex-font-style-bf">only immediately after</span> getting to time $b_k$ and learning that he was supposed to complete the $k$-th task at time $a_k$. That is, even if Okabe already had to perform $k$-th task before, he wouldn't remember it before stumbling on the info about this task at time $b_k$ again.</p></li></ul><p>Please refer to the notes for an example of time travelling.</p><p>There is a certain set $s$ of tasks such that the first moment that all of the tasks in $s$ are simultaneously completed (regardless of whether any other tasks are currently completed), a funny scene will take place. Omkar loves this scene and wants to know how many times Okabe will time travel before this scene takes place. Find this number modulo $10^9 + 7$. It can be proven that eventually all $n$ tasks will be completed and so the answer always exists.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) &nbsp;— the number of tasks that Okabe needs to complete.</p><p>$n$ lines follow. The $k$-th of these lines contain two integers $a_k$ and $b_k$ ($1 \leq a_k &lt; b_k \leq 2n$) &nbsp;— the time at which Okabe needs to complete the $k$-th task and the time that he realizes this respectively. All $2n$ of these times are distinct (so every time from $1$ to $2n$ inclusive appears exactly once in the input).</p><p>The next line contains a single integer $t$ ($1 \leq t \leq n$) &nbsp;— the size of the set $s$ of tasks that lead to the funny scene.</p><p>The last line contains $t$ integers $s_1, s_2, \ldots, s_t$ &nbsp;— ($1 \leq s_k \leq n$, the numbers $s_1, s_2, \ldots, s_t$ are distinct) &nbsp;— the set $s$ of tasks.</p></div><div class="output-specification"><p>Output a single integer &nbsp;— the number of times that Okabe time travels until all tasks in the set $s$ are simultaneously completed, modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \leq n \leq 2 \cdot 10^5$) &nbsp;— the number of tasks that Okabe needs to complete.</p><p>$n$ lines follow. The $k$-th of these lines contain two integers $a_k$ and $b_k$ ($1 \leq a_k &lt; b_k \leq 2n$) &nbsp;— the time at which Okabe needs to complete the $k$-th task and the time that he realizes this respectively. All $2n$ of these times are distinct (so every time from $1$ to $2n$ inclusive appears exactly once in the input).</p><p>The next line contains a single integer $t$ ($1 \leq t \leq n$) &nbsp;— the size of the set $s$ of tasks that lead to the funny scene.</p><p>The last line contains $t$ integers $s_1, s_2, \ldots, s_t$ &nbsp;— ($1 \leq s_k \leq n$, the numbers $s_1, s_2, \ldots, s_t$ are distinct) &nbsp;— the set $s$ of tasks.</p>

## Output

<p>Output a single integer &nbsp;— the number of times that Okabe time travels until all tasks in the set $s$ are simultaneously completed, modulo $10^9 + 7$.</p>





```input1
2
1 4
2 3
2
1 2
```




```input2
2
1 4
2 3
1
1
```




```input3
1
1 2
1
1
```




```input4
6
10 12
3 7
4 6
2 9
5 8
1 11
3
2 4 6
```




```input5
16
31 32
3 26
17 19
4 24
1 28
15 21
12 16
18 29
20 23
7 8
11 14
9 22
6 30
5 10
25 27
2 13
6
3 8 2 5 12 11
```




```output1
3
```




```output2
2
```




```output3
1
```




```output4
17
```




```output5
138
```



## Note

<p>For the first sample, all tasks need to be completed in order for the funny scene to occur.</p><p>Initially, the time is $0$. Nothing happens until time $3$, when Okabe realizes that he should have done the $2$-nd task at time $2$. He then time travels to time $2$ and completes the task.</p><p>As the task is done now, he does not time travel again when the time is again $3$. However, at time $4$, he travels to time $1$ to complete the $1$-st task.</p><p>This undoes the $2$-nd task. This means that the $2$-nd task is not currently completed, meaning that the funny scene will <span class="tex-font-style-bf">not</span> occur at this point even though the $1$-st task is currently completed and Okabe had previously completed the $2$-nd task.</p><p>Once it is again time $3$ he travels back to time $2$ once more and does the $2$-nd task again.</p><p>Now all tasks are complete, with Okabe having time travelled $3$ times.</p><p>The second sample has the same tasks for Okabe to complete. However, this time the funny scene only needs the first task to be completed in order to occur. From reading the above sample you can see that this occurs once Okabe has time travelled $2$ times.</p>
