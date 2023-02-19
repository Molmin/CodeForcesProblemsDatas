## Description

<div><p>There is the faculty of Computer Science in Berland. In the social net "TheContact!" for each course of this faculty there is the special group whose name equals the year of university entrance of corresponding course of students at the university. </p><p>Each of students joins the group of his course and joins all groups for which the year of student's university entrance differs by no more than <span class="tex-span"><i>x</i></span> from the year of university entrance of this student, where <span class="tex-span"><i>x</i></span> — some non-negative integer. A value <span class="tex-span"><i>x</i></span> is not given, but it can be uniquely determined from the available data. Note that students don't join other groups. </p><p>You are given the list of groups which the student Igor joined. According to this information you need to determine the year of Igor's university entrance.</p></div><div class="input-specification"><p>The first line contains the positive odd integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5</span>) — the number of groups which Igor joined. </p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2010 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2100</span>) — years of student's university entrance for each group in which Igor is the member.</p><p>It is guaranteed that the input data is correct and the answer always exists. Groups are given randomly.</p></div><div class="output-specification"><p>Print the year of Igor's university entrance. </p></div>

## Input

<p>The first line contains the positive odd integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5</span>) — the number of groups which Igor joined. </p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2010 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2100</span>) — years of student's university entrance for each group in which Igor is the member.</p><p>It is guaranteed that the input data is correct and the answer always exists. Groups are given randomly.</p>

## Output

<p>Print the year of Igor's university entrance. </p>





```input1
3
2014 2016 2015

```




```input2
1
2050

```




```output1
2015

```




```output2
2050

```



## Note

<p>In the first test the value <span class="tex-span"><i>x</i> = 1</span>. Igor entered the university in 2015. So he joined groups members of which are students who entered the university in 2014, 2015 and 2016.</p><p>In the second test the value <span class="tex-span"><i>x</i> = 0</span>. Igor entered only the group which corresponds to the year of his university entrance. </p>
