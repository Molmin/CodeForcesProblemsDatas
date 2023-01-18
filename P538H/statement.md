## Description

<div><p><span class="tex-span"><i>T</i></span> students applied into the ZPP class of Summer Irrelevant School. The organizing committee of the school may enroll any number of them, but at least <span class="tex-span"><i>t</i></span> students must be enrolled. The enrolled students should be divided into two groups in any manner (it is possible that one of the groups will be empty!)</p><p>During a shift the students from the ZPP grade are tutored by <span class="tex-span"><i>n</i></span> teachers. Due to the nature of the educational process, each of the teachers should be assigned to exactly one of two groups (it is possible that no teacher will be assigned to some of the groups!). The <span class="tex-span"><i>i</i></span>-th teacher is willing to work in a group as long as the group will have at least <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and at most <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> students (otherwise it would be either too boring or too hard). Besides, some pairs of the teachers don't like each other other and therefore can not work in the same group; in total there are <span class="tex-span"><i>m</i></span> pairs of conflicting teachers.</p><p>You, as the head teacher of Summer Irrelevant School, have got a difficult task: to determine how many students to enroll in each of the groups and in which group each teacher will teach.</p></div><div class="input-specification"><p>The first line contains two space-separated integers, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines describe the pairs of conflicting teachers. Each of these lines contain two space-separated integers — the indices of teachers in the pair. The teachers are indexed starting from one. It is guaranteed that no teacher has a conflict with himself and no pair of conflicting teachers occurs in the list more than once.</p></div><div class="output-specification"><p>If the distribution is possible, print in the first line a single word '<span class="tex-font-style-tt">POSSIBLE</span>' (without the quotes). In the second line print two space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>&nbsp;— the number of students in the first and second group, correspondingly, the contstraint <span class="tex-span"><i>t</i> ≤ <i>n</i><sub class="lower-index">1</sub> + <i>n</i><sub class="lower-index">2</sub> ≤ <i>T</i></span> should be met. In the third line print <span class="tex-span"><i>n</i></span> characters, the <span class="tex-span"><i>i</i></span>-th of which should be 1 or 2, if the <span class="tex-span"><i>i</i></span>-th teacher should be assigned to the first or second group, correspondingly. If there are multiple possible distributions of students and teachers in groups, you can print any of them.</p><p>If the sought distribution doesn't exist, print a single word '<span class="tex-font-style-tt">IMPOSSIBLE</span>' (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated integers, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ <i>T</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines describe the pairs of conflicting teachers. Each of these lines contain two space-separated integers — the indices of teachers in the pair. The teachers are indexed starting from one. It is guaranteed that no teacher has a conflict with himself and no pair of conflicting teachers occurs in the list more than once.</p>

## Output

<p>If the distribution is possible, print in the first line a single word '<span class="tex-font-style-tt">POSSIBLE</span>' (without the quotes). In the second line print two space-separated integers <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>&nbsp;— the number of students in the first and second group, correspondingly, the contstraint <span class="tex-span"><i>t</i> ≤ <i>n</i><sub class="lower-index">1</sub> + <i>n</i><sub class="lower-index">2</sub> ≤ <i>T</i></span> should be met. In the third line print <span class="tex-span"><i>n</i></span> characters, the <span class="tex-span"><i>i</i></span>-th of which should be 1 or 2, if the <span class="tex-span"><i>i</i></span>-th teacher should be assigned to the first or second group, correspondingly. If there are multiple possible distributions of students and teachers in groups, you can print any of them.</p><p>If the sought distribution doesn't exist, print a single word '<span class="tex-font-style-tt">IMPOSSIBLE</span>' (without the quotes).</p>





```input1
10 20
3 0
3 6
4 9
16 25

```




```input2
1 10
3 3
0 10
0 10
0 10
1 2
1 3
2 3

```




```output1
POSSIBLE
4 16
112

```




```output2
IMPOSSIBLE

```


