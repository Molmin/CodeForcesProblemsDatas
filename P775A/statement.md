## Description

<div><p>In this problem your task is to come up with a week schedule of classes in university for professors and student groups. Consider that there are <span class="tex-span">6</span> educational days in week and maximum number of classes per educational day is <span class="tex-span">7</span> (classes numerated from <span class="tex-span">1</span> to <span class="tex-span">7</span> for each educational day).</p><p>It is known that in university <span class="tex-span"><i>n</i></span> students study, <span class="tex-span"><i>m</i></span> professors work and there are <span class="tex-span"><i>a</i></span> classrooms for conducting classes. Also you have two-dimensional array with <span class="tex-span"><i>n</i> × <i>m</i></span> size which contains the following information. The number which stays in <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column equals to the number of classes which professor <span class="tex-span"><i>j</i></span> must conduct with the group <span class="tex-span"><i>i</i></span> in a single week. The schedule which you output must satisfy to array described above.</p><p>There are several other conditions for schedule. Single professor can not conduct more than one class. Similarly, single student group can not be on more than one class at the same time.</p><p>Let define a <span class="tex-font-style-it">fatigue</span> function for professors and student groups. Call this function <span class="tex-span"><i>f</i></span>.</p><p>To single professor <span class="tex-font-style-it">fatigue</span> calculated in the following way. Let look on classes which this professor must conduct in each of the <span class="tex-span">6</span>-th educational days. Let <span class="tex-span"><i>x</i></span> be the number of class which professor will firstly conduct in day <span class="tex-span"><i>i</i></span> and let <span class="tex-span"><i>y</i></span> — the last class for this professor. Then the value <span class="tex-span">(2 + <i>y</i> - <i>x</i> + 1)·(2 + <i>y</i> - <i>x</i> + 1)</span> must be added to professor's <span class="tex-font-style-it">fatigue</span>. If professor has no classes in day <span class="tex-span"><i>i</i></span>, nothing is added to professor's <span class="tex-font-style-it">fatigue</span>. </p><p>For single student group <span class="tex-font-style-it">fatigue</span> is calculated similarly. Lets look at classes of this group in each of the <span class="tex-span">6</span> educational days. Let <span class="tex-span"><i>x</i></span> be the number of first class for this group on day <span class="tex-span"><i>i</i></span> and let <span class="tex-span"><i>y</i></span> — the last class for this group. Then the value <span class="tex-span">(2 + <i>y</i> - <i>x</i> + 1)·(2 + <i>y</i> - <i>x</i> + 1)</span> must be added to this group's <span class="tex-font-style-it">fatigue</span>. If student group has no classes in day <span class="tex-span"><i>i</i></span>, nothing is added to group's <span class="tex-font-style-it">fatigue</span>.</p><p>So the value of function <span class="tex-span"><i>f</i></span> equals to total {fatigue} for all <span class="tex-span"><i>n</i></span> student groups and for all <span class="tex-span"><i>m</i></span> professors.</p><p>Your task is to come up with such a schedule which minimizes the value of function <span class="tex-span"><i>f</i></span>.</p><p>Jury prepared some solution of this problem. For each test you will get a certain number of points. It equals to result of division of the value of function <span class="tex-span"><i>f</i></span> from the jury solution by the value of function <span class="tex-span"><i>f</i></span> for schedule which your program output (i. e. the smaller value of {fatigue} function your program find the more points you will get), multiplied by <span class="tex-span">100</span>. In the other words if the value of <span class="tex-span"><i>f</i></span> for jury solution equals to <span class="tex-span"><i>p</i></span> and for your solution — to <span class="tex-span"><i>q</i></span>, you will get <span class="tex-span">100·<i>p</i> / <i>q</i></span> points (note, that the number of points is a real number). The points will be added together for all tests. The goal is to score as many points as possible. </p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>a</i> ≤ 60</span>) — the number of groups, the number of professors and the number of classrooms.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers from <span class="tex-span">0</span> to <span class="tex-span">24</span> — <span class="tex-span"><i>j</i></span>-th number in <span class="tex-span"><i>i</i></span>-th line equals to the number of classes with the professor <span class="tex-span"><i>j</i></span> must conduct with the <span class="tex-span"><i>i</i></span>-th student group.</p><p>It is guaranteed that the number of classes in week for each professor and for each student group does not exceed <span class="tex-span">24</span>. Also guaranteed that the total number of classes in week does not exceed <span class="tex-span">75</span>% from a maximum number of classes which can be conducted based on the number of classrooms. For all tests there is at least one schedule satisfying all described conditions.</p></div><div class="output-specification"><p>In the first line print the minimized value of function <span class="tex-span"><i>f</i></span>.</p><p>After that print blank line.</p><p>After that print the schedule for each student group in increasing order of group number. For each student group print <span class="tex-span">7</span> lines. Each line must contains <span class="tex-span">6</span> numbers. Let the number at <span class="tex-span"><i>i</i></span>-th line and <span class="tex-span"><i>j</i></span>-th column equals to <span class="tex-span"><i>x</i></span>. If in <span class="tex-span"><i>j</i></span>-th day current group has no class number <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>x</i></span> must be equals to zero. Otherwise <span class="tex-span"><i>x</i></span> must be equals to the number of professor who will conduct the corresponding class with the corresponding student group. </p><p>The number of classes which will be conducted simultaneously must not exceeds the number of classrooms <span class="tex-span"><i>a</i></span>.</p><p>Separate the description of the schedules for groups with a blank line.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>a</i> ≤ 60</span>) — the number of groups, the number of professors and the number of classrooms.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> integers from <span class="tex-span">0</span> to <span class="tex-span">24</span> — <span class="tex-span"><i>j</i></span>-th number in <span class="tex-span"><i>i</i></span>-th line equals to the number of classes with the professor <span class="tex-span"><i>j</i></span> must conduct with the <span class="tex-span"><i>i</i></span>-th student group.</p><p>It is guaranteed that the number of classes in week for each professor and for each student group does not exceed <span class="tex-span">24</span>. Also guaranteed that the total number of classes in week does not exceed <span class="tex-span">75</span>% from a maximum number of classes which can be conducted based on the number of classrooms. For all tests there is at least one schedule satisfying all described conditions.</p>

## Output

<p>In the first line print the minimized value of function <span class="tex-span"><i>f</i></span>.</p><p>After that print blank line.</p><p>After that print the schedule for each student group in increasing order of group number. For each student group print <span class="tex-span">7</span> lines. Each line must contains <span class="tex-span">6</span> numbers. Let the number at <span class="tex-span"><i>i</i></span>-th line and <span class="tex-span"><i>j</i></span>-th column equals to <span class="tex-span"><i>x</i></span>. If in <span class="tex-span"><i>j</i></span>-th day current group has no class number <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>x</i></span> must be equals to zero. Otherwise <span class="tex-span"><i>x</i></span> must be equals to the number of professor who will conduct the corresponding class with the corresponding student group. </p><p>The number of classes which will be conducted simultaneously must not exceeds the number of classrooms <span class="tex-span"><i>a</i></span>.</p><p>Separate the description of the schedules for groups with a blank line.</p>





```input1
3 3 1
1 0 0
0 1 0
0 0 1

```




```input2
3 1 1
1
1
1

```




```input3
5 7 10
1 3 6 0 1 2 4
0 3 0 6 5 1 4
3 5 1 2 3 2 4
2 3 1 1 4 1 2
2 4 3 2 4 3 2

```




```output1
54

1 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

0 0 0 0 0 0 
2 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

0 0 0 0 0 0 
0 0 0 0 0 0 
3 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

```




```output2
52

1 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

0 0 0 0 0 0 
1 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

0 0 0 0 0 0 
0 0 0 0 0 0 
1 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

```




```output3
1512

0 0 6 0 0 2 
0 7 6 3 3 7 
3 1 2 3 2 7 
3 7 0 0 0 0 
5 3 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

0 0 4 0 7 6 
4 5 7 4 5 5 
7 2 4 4 5 5 
7 2 0 4 0 0 
0 2 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

4 0 7 2 5 7 
5 0 2 5 7 1 
2 4 1 2 7 1 
2 3 0 0 0 0 
0 6 0 0 0 0 
0 6 0 0 0 0 
0 0 0 0 0 0 

0 0 0 5 3 5 
0 2 4 7 2 6 
0 5 7 0 0 0 
1 5 1 0 0 0 
2 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

0 0 5 7 2 3 
0 1 3 2 6 3 
5 7 6 5 6 4 
5 4 2 2 0 0 
1 0 0 0 0 0 
0 0 0 0 0 0 
0 0 0 0 0 0 

```



## Note

<p>During the main part of the competition (one week) you solution will be judged on <span class="tex-span">100</span> preliminary tests. The first <span class="tex-span">10</span> preliminary tests are available for download by a link <a href="//assets.codeforces.com/files/vk/vkcup-2017-wr2-materials-v1.tar.gz">http://assets.codeforces.com/files/vk/vkcup-2017-wr2-materials-v1.tar.gz</a>.</p><p>After the end of the contest (i.e., a week after its start) the last solution you sent (having positive score) will be chosen to be launched on the extended final tests.</p>
