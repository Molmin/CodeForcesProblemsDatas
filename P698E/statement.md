## Description

<div><p>Sometime the classic solution are not powerful enough and we have to design our own. For the purpose of this problem you have to implement the part of the system of task scheduling.</p><p>Each task should be executed at some particular moments of time. In our system you may set the exact value for the second, minute, hour, day of the week, day and month, when the task should be executed. Moreover, one can set a special value <span class="tex-font-style-tt">-1</span> that means any value of this parameter is valid.</p><p>For example, if the parameter string is <span class="tex-font-style-tt">-1 59 23 -1 -1 -1</span>, the problem will be executed every day at 23:59:00, 23:59:01, 23:59:02, ..., 23:59:59 (<span class="tex-span">60</span> times in total).</p><p>Seconds, minutes and hours are numbered starting from zero, while day, months and days of the week are numbered starting from one. The first day of the week is Monday.</p><p>There is one special case that is treated separately. If both day of the week and day are given (i.e. differ from <span class="tex-font-style-tt">-1</span>) to execute the task only one of these two (at least one, if both match this is fine too) parameters should match the current time (of course, all other parameters should match too). For example, the string of parameters <span class="tex-font-style-tt">0 0 12 6 3 7</span> means that the task will be executed both on Saturday, July 2nd, 2016 and on Sunday, July 3rd, 2016 at noon.</p><p>One should not forget about the existence of the leap years. The year is leap if it's number is divisible by <span class="tex-span">400</span>, or is not divisible by <span class="tex-span">100</span>, but is divisible by <span class="tex-span">4</span>. Each leap year has 366 days instead of usual 365, by extending February to 29 days rather than the common 28.</p><p>The current time is represented as the number of seconds passed after 00:00:00 January 1st, 1970 (Thursday).</p><p>You are given the string of six parameters, describing the moments of time the task should be executed. You are also given a number of moments of time. For each of them you have to find the first moment of time strictly greater than the current when the task will be executed.</p></div><div class="input-specification"><p>The first line of the input contains six integers <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>day</i></span>, <span class="tex-span"><i>date</i></span> and <span class="tex-span"><i>month</i></span> (<span class="tex-span">0 ≤ <i>s</i>, <i>m</i> ≤ 59</span>, <span class="tex-span">0 ≤ <i>h</i> ≤ 23</span>, <span class="tex-span">1 ≤ <i>day</i> ≤ 7</span>, <span class="tex-span">1 ≤ <i>date</i> ≤ 31</span>, <span class="tex-span">1 ≤ <i>month</i> ≤ 12</span>). Each of the number can also be equal to <span class="tex-span"> - 1</span>. It's guaranteed, that there are infinitely many moments of time when this task should be executed.</p><p>Next line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of moments of time you have to solve the problem for. Each of the next <span class="tex-span"><i>n</i></span> lines contains a single integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain the first moment of time strictly greater than <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, when the task should be executed.</p></div>

## Input

<p>The first line of the input contains six integers <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>day</i></span>, <span class="tex-span"><i>date</i></span> and <span class="tex-span"><i>month</i></span> (<span class="tex-span">0 ≤ <i>s</i>, <i>m</i> ≤ 59</span>, <span class="tex-span">0 ≤ <i>h</i> ≤ 23</span>, <span class="tex-span">1 ≤ <i>day</i> ≤ 7</span>, <span class="tex-span">1 ≤ <i>date</i> ≤ 31</span>, <span class="tex-span">1 ≤ <i>month</i> ≤ 12</span>). Each of the number can also be equal to <span class="tex-span"> - 1</span>. It's guaranteed, that there are infinitely many moments of time when this task should be executed.</p><p>Next line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of moments of time you have to solve the problem for. Each of the next <span class="tex-span"><i>n</i></span> lines contains a single integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain the first moment of time strictly greater than <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, when the task should be executed.</p>





```input1
-1 59 23 -1 -1 -1
6
1467372658
1467417540
1467417541
1467417598
1467417599
1467417600

```




```input2
0 0 12 6 3 7
3
1467372658
1467460810
1467547200

```




```output1
1467417540
1467417541
1467417542
1467417599
1467503940
1467503940

```




```output2
1467460800
1467547200
1468065600

```



## Note

<p>The moment of time <span class="tex-span">1467372658</span> after the midnight of January 1st, 1970 is 11:30:58 July 1st, 2016.</p>
