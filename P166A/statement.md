## Description

<div><p>Another programming contest is over. You got hold of the contest's final results table. The table has the following data. For each team we are shown two numbers: the number of problems and the total penalty time. However, for no team we are shown its final place.</p><p>You know the rules of comparing the results of two given teams very well. Let's say that team <span class="tex-span"><i>a</i></span> solved <span class="tex-span"><i>p</i><sub class="lower-index"><i>a</i></sub></span> problems with total penalty time <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span> and team <span class="tex-span"><i>b</i></span> solved <span class="tex-span"><i>p</i><sub class="lower-index"><i>b</i></sub></span> problems with total penalty time <span class="tex-span"><i>t</i><sub class="lower-index"><i>b</i></sub></span>. Team <span class="tex-span"><i>a</i></span> gets a higher place than team <span class="tex-span"><i>b</i></span> in the end, if it either solved more problems on the contest, or solved the same number of problems but in less total time. In other words, team <span class="tex-span"><i>a</i></span> gets a higher place than team <span class="tex-span"><i>b</i></span> in the final results' table if either <span class="tex-span"><i>p</i><sub class="lower-index"><i>a</i></sub> &gt; <i>p</i><sub class="lower-index"><i>b</i></sub></span>, or <span class="tex-span"><i>p</i><sub class="lower-index"><i>a</i></sub> = <i>p</i><sub class="lower-index"><i>b</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub> &lt; <i>t</i><sub class="lower-index"><i>b</i></sub></span>. </p><p>It is considered that the teams that solve the same number of problems with the same penalty time share all corresponding places. More formally, let's say there is a group of <span class="tex-span"><i>x</i></span> teams that solved the same number of problems with the same penalty time. Let's also say that <span class="tex-span"><i>y</i></span> teams performed better than the teams from this group. In this case all teams from the group share places <span class="tex-span"><i>y</i> + 1</span>, <span class="tex-span"><i>y</i> + 2</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>y</i> + <i>x</i></span>. The teams that performed worse than the teams from this group, get their places in the results table starting from the <span class="tex-span"><i>y</i> + <i>x</i> + 1</span>-th place.</p><p>Your task is to count what number of teams from the given list shared the <span class="tex-span"><i>k</i></span>-th place. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 50</span>). Then <span class="tex-span"><i>n</i></span> lines contain the description of the teams: the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>) — the number of solved problems and the total penalty time of the <span class="tex-span"><i>i</i></span>-th team, correspondingly. All numbers in the lines are separated by spaces. </p></div><div class="output-specification"><p>In the only line print the sought number of teams that got the <span class="tex-span"><i>k</i></span>-th place in the final results' table.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 50</span>). Then <span class="tex-span"><i>n</i></span> lines contain the description of the teams: the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 50</span>) — the number of solved problems and the total penalty time of the <span class="tex-span"><i>i</i></span>-th team, correspondingly. All numbers in the lines are separated by spaces. </p>

## Output

<p>In the only line print the sought number of teams that got the <span class="tex-span"><i>k</i></span>-th place in the final results' table.</p>





```input1
7 2
4 10
4 10
4 10
3 20
2 1
2 1
1 10

```




```input2
5 4
3 1
3 1
5 3
3 1
3 1

```




```output1
3

```




```output2
4

```



## Note

<p>The final results' table for the first sample is: </p><ul> <li> 1-3 places — 4 solved problems, the penalty time equals 10 </li><li> 4 place — 3 solved problems, the penalty time equals 20 </li><li> 5-6 places — 2 solved problems, the penalty time equals 1 </li><li> 7 place — 1 solved problem, the penalty time equals 10 </li></ul><p>The table shows that the second place is shared by the teams that solved 4 problems with penalty time 10. There are 3 such teams.</p><p>The final table for the second sample is:</p><ul> <li> 1 place — 5 solved problems, the penalty time equals 3 </li><li> 2-5 places — 3 solved problems, the penalty time equals 1 </li></ul><p>The table shows that the fourth place is shared by the teams that solved 3 problems with penalty time 1. There are 4 such teams.</p>
