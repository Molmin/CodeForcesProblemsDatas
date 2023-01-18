## Description

<div><p>Tomorrow Peter has a Biology exam. He does not like this subject much, but <span class="tex-span"><i>d</i></span> days ago he learnt that he would have to take this exam. Peter's strict parents made him prepare for the exam immediately, for this purpose he has to study not less than <span class="tex-span"><i>minTime</i><sub class="lower-index"><i>i</i></sub></span> and not more than <span class="tex-span"><i>maxTime</i><sub class="lower-index"><i>i</i></sub></span> hours per each <span class="tex-span"><i>i</i></span>-th day. Moreover, they warned Peter that a day before the exam they would check how he has followed their instructions.</p><p>So, today is the day when Peter's parents ask him to show the timetable of his preparatory studies. But the boy has counted only the sum of hours <span class="tex-span"><i>sumTime</i></span> spent him on preparation, and now he wants to know if he can show his parents a timetable <span class="tex-span"><i>sсhedule</i></span> with <span class="tex-span"><i>d</i></span> numbers, where each number <span class="tex-span"><i>sсhedule</i><sub class="lower-index"><i>i</i></sub></span> stands for the time in hours spent by Peter each <span class="tex-span"><i>i</i></span>-th day on biology studies, and satisfying the limitations imposed by his parents, and at the same time the sum total of all <span class="tex-span"><i>schedule</i><sub class="lower-index"><i>i</i></sub></span> should equal to <span class="tex-span"><i>sumTime</i></span>.</p></div><div class="input-specification"><p>The first input line contains two integer numbers <span class="tex-span"><i>d</i>, <i>sumTime</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ 30, 0 ≤ <i>sumTime</i> ≤ 240</span>) — the amount of days, during which Peter studied, and the total amount of hours, spent on preparation. Each of the following <span class="tex-span"><i>d</i></span> lines contains two integer numbers <span class="tex-span"><i>minTime</i><sub class="lower-index"><i>i</i></sub>, <i>maxTime</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>minTime</i><sub class="lower-index"><i>i</i></sub> ≤ <i>maxTime</i><sub class="lower-index"><i>i</i></sub> ≤ 8</span>), separated by a space — minimum and maximum amount of hours that Peter could spent in the <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>In the first line print <span class="tex-font-style-tt">YES</span>, and in the second line print <span class="tex-span"><i>d</i></span> numbers (separated by a space), each of the numbers — amount of hours, spent by Peter on preparation in the corresponding day, if he followed his parents' instructions; or print <span class="tex-font-style-tt">NO</span> in the unique line. If there are many solutions, print any of them.</p></div>

## Input

<p>The first input line contains two integer numbers <span class="tex-span"><i>d</i>, <i>sumTime</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ 30, 0 ≤ <i>sumTime</i> ≤ 240</span>) — the amount of days, during which Peter studied, and the total amount of hours, spent on preparation. Each of the following <span class="tex-span"><i>d</i></span> lines contains two integer numbers <span class="tex-span"><i>minTime</i><sub class="lower-index"><i>i</i></sub>, <i>maxTime</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>minTime</i><sub class="lower-index"><i>i</i></sub> ≤ <i>maxTime</i><sub class="lower-index"><i>i</i></sub> ≤ 8</span>), separated by a space — minimum and maximum amount of hours that Peter could spent in the <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>In the first line print <span class="tex-font-style-tt">YES</span>, and in the second line print <span class="tex-span"><i>d</i></span> numbers (separated by a space), each of the numbers — amount of hours, spent by Peter on preparation in the corresponding day, if he followed his parents' instructions; or print <span class="tex-font-style-tt">NO</span> in the unique line. If there are many solutions, print any of them.</p>





```input1
1 48
5 7

```




```input2
2 5
0 1
3 5

```




```output1
NO

```




```output2
YES
1 4
```


