## Description

<div><p>Ivan is a student at Berland State University (BSU). There are <span class="tex-span"><i>n</i></span> days in Berland week, and each of these days Ivan might have some classes at the university.</p><p>There are <span class="tex-span"><i>m</i></span> working hours during each Berland day, and each lesson at the university lasts exactly one hour. If at some day Ivan's first lesson is during <span class="tex-span"><i>i</i></span>-th hour, and last lesson is during <span class="tex-span"><i>j</i></span>-th hour, then he spends <span class="tex-span"><i>j</i> - <i>i</i> + 1</span> hours in the university during this day. If there are no lessons during some day, then Ivan stays at home and therefore spends <span class="tex-span">0</span> hours in the university.</p><p>Ivan doesn't like to spend a lot of time in the university, so he has decided to skip some lessons. He cannot skip more than <span class="tex-span"><i>k</i></span> lessons during the week. After deciding which lessons he should skip and which he should attend, every day Ivan will enter the university right before the start of the first lesson he does not skip, and leave it after the end of the last lesson he decides to attend. If Ivan skips all lessons during some day, he doesn't go to the university that day at all.</p><p>Given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> and Ivan's timetable, can you determine the minimum number of hours he has to spend in the university during one week, if he cannot skip more than <span class="tex-span"><i>k</i></span> lessons?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 500</span>) — the number of days in the Berland week, the number of working hours during each day, and the number of lessons Ivan can skip, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing a binary string of <span class="tex-span"><i>m</i></span> characters. If <span class="tex-span"><i>j</i></span>-th character in <span class="tex-span"><i>i</i></span>-th line is <span class="tex-font-style-tt">1</span>, then Ivan has a lesson on <span class="tex-span"><i>i</i></span>-th day during <span class="tex-span"><i>j</i></span>-th hour (if it is <span class="tex-font-style-tt">0</span>, there is no such lesson).</p></div><div class="output-specification"><p>Print the minimum number of hours Ivan has to spend in the university during the week if he skips not more than <span class="tex-span"><i>k</i></span> lessons.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 500</span>) — the number of days in the Berland week, the number of working hours during each day, and the number of lessons Ivan can skip, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing a binary string of <span class="tex-span"><i>m</i></span> characters. If <span class="tex-span"><i>j</i></span>-th character in <span class="tex-span"><i>i</i></span>-th line is <span class="tex-font-style-tt">1</span>, then Ivan has a lesson on <span class="tex-span"><i>i</i></span>-th day during <span class="tex-span"><i>j</i></span>-th hour (if it is <span class="tex-font-style-tt">0</span>, there is no such lesson).</p>

## Output

<p>Print the minimum number of hours Ivan has to spend in the university during the week if he skips not more than <span class="tex-span"><i>k</i></span> lessons.</p>





```input1
2 5 1
01001
10110

```




```input2
2 5 0
01001
10110

```




```output1
5

```




```output2
8

```



## Note

<p>In the first example Ivan can skip any of two lessons during the first day, so he spends <span class="tex-span">1</span> hour during the first day and <span class="tex-span">4</span> hours during the second day.</p><p>In the second example Ivan can't skip any lessons, so he spends <span class="tex-span">4</span> hours every day.</p>
