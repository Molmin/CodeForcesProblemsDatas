## Description

<div><p>Soon there will be held the world's largest programming contest, but the testing system still has <span class="tex-span"><i>m</i></span> bugs. The contest organizer, a well-known university, has no choice but to attract university students to fix all the bugs. The university has <span class="tex-span"><i>n</i></span> students able to perform such work. The students realize that they are the only hope of the organizers, so they don't want to work for free: the <span class="tex-span"><i>i</i></span>-th student wants to get <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> 'passes' in his subjects (regardless of the volume of his work).</p><p>Bugs, like students, are not the same: every bug is characterized by complexity <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, and every student has the level of his abilities <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Student <span class="tex-span"><i>i</i></span> can fix a bug <span class="tex-span"><i>j</i></span> only if the level of his abilities is not less than the complexity of the bug: <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>j</i></sub></span>, and he does it in one day. Otherwise, the bug will have to be fixed by another student. Of course, no student can work on a few bugs in one day. All bugs are not dependent on each other, so they can be corrected in any order, and different students can work simultaneously.</p><p>The university wants to fix all the bugs as quickly as possible, but giving the students the total of not more than <span class="tex-span"><i>s</i></span> passes. Determine which students to use for that and come up with the schedule of work saying which student should fix which bug.</p></div><div class="input-specification"><p>The first line contains three space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of students, the number of bugs in the system and the maximum number of passes the university is ready to give the students.</p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>,&nbsp;..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the bugs' complexities.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>,&nbsp;..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the levels of the students' abilities.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>,&nbsp;..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the numbers of the passes the students want to get for their help.</p></div><div class="output-specification"><p>If the university can't correct all bugs print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, on the first line print "<span class="tex-font-style-tt">YES</span>", and on the next line print <span class="tex-span"><i>m</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th of these numbers should equal the number of the student who corrects the <span class="tex-span"><i>i</i></span>-th bug in the optimal answer. The bugs should be corrected as quickly as possible (you must spend the minimum number of days), and the total given passes mustn't exceed <span class="tex-span"><i>s</i></span>. If there are multiple optimal answers, you can output any of them.</p></div>

## Input

<p>The first line contains three space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of students, the number of bugs in the system and the maximum number of passes the university is ready to give the students.</p><p>The next line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>,&nbsp;..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the bugs' complexities.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>,&nbsp;..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the levels of the students' abilities.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>,&nbsp;..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the numbers of the passes the students want to get for their help.</p>

## Output

<p>If the university can't correct all bugs print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, on the first line print "<span class="tex-font-style-tt">YES</span>", and on the next line print <span class="tex-span"><i>m</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th of these numbers should equal the number of the student who corrects the <span class="tex-span"><i>i</i></span>-th bug in the optimal answer. The bugs should be corrected as quickly as possible (you must spend the minimum number of days), and the total given passes mustn't exceed <span class="tex-span"><i>s</i></span>. If there are multiple optimal answers, you can output any of them.</p>





```input1
3 4 9
1 3 1 2
2 1 3
4 3 6

```




```input2
3 4 10
2 3 1 2
2 1 3
4 3 6

```




```input3
3 4 9
2 3 1 2
2 1 3
4 3 6

```




```input4
3 4 5
1 3 1 2
2 1 3
5 3 6

```




```output1
YES
2 3 2 3

```




```output2
YES
1 3 1 3

```




```output3
YES
3 3 2 3

```




```output4
NO

```



## Note

<p>Consider the first sample.</p><p>The third student (with level 3) must fix the 2nd and 4th bugs (complexities 3 and 2 correspondingly) and the second student (with level 1) must fix the 1st and 3rd bugs (their complexity also equals 1). Fixing each bug takes one day for each student, so it takes 2 days to fix all bugs (the students can work in parallel).</p><p>The second student wants 3 passes for his assistance, the third student wants 6 passes. It meets the university's capabilities as it is ready to give at most 9 passes.</p>
