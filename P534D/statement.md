## Description

<div><p>On February, 30th <span class="tex-span"><i>n</i></span> students came in the Center for Training Olympiad Programmers (CTOP) of the Berland State University. They came one by one, one after another. Each of them went in, and before sitting down at his desk, greeted with those who were present in the room by shaking hands. Each of the students who came in stayed in CTOP until the end of the day and never left.</p><p>At any time any three students could join together and start participating in a team contest, which lasted until the end of the day. The team did not distract from the contest for a minute, so when another student came in and greeted those who were present, he did not shake hands with the members of the contest writing team. Each team consisted of exactly three students, and each student could not become a member of more than one team. Different teams could start writing contest at different times.</p><p>Given how many present people shook the hands of each student, get a possible order in which the students could have come to CTOP. If such an order does not exist, then print that this is impossible.</p><p>Please note that some students could work independently until the end of the day, without participating in a team contest.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of students who came to CTOP. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of students with who the <span class="tex-span"><i>i</i></span>-th student shook hands.</p></div><div class="output-specification"><p>If the sought order of students exists, print in the first line "<span class="tex-font-style-tt">Possible</span>" and in the second line print the permutation of the students' numbers defining the order in which the students entered the center. Number <span class="tex-span"><i>i</i></span> that stands to the left of number <span class="tex-span"><i>j</i></span> in this permutation means that the <span class="tex-span"><i>i</i></span>-th student came earlier than the <span class="tex-span"><i>j</i></span>-th student. If there are multiple answers, print any of them.</p><p>If the sought order of students doesn't exist, in a single line print "<span class="tex-font-style-tt">Impossible</span>".</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of students who came to CTOP. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of students with who the <span class="tex-span"><i>i</i></span>-th student shook hands.</p>

## Output

<p>If the sought order of students exists, print in the first line "<span class="tex-font-style-tt">Possible</span>" and in the second line print the permutation of the students' numbers defining the order in which the students entered the center. Number <span class="tex-span"><i>i</i></span> that stands to the left of number <span class="tex-span"><i>j</i></span> in this permutation means that the <span class="tex-span"><i>i</i></span>-th student came earlier than the <span class="tex-span"><i>j</i></span>-th student. If there are multiple answers, print any of them.</p><p>If the sought order of students doesn't exist, in a single line print "<span class="tex-font-style-tt">Impossible</span>".</p>





```input1
5
2 1 3 0 1

```




```input2
9
0 2 3 4 1 1 0 2 2

```




```input3
4
0 2 1 1

```




```output1
Possible
4 5 1 3 2
```




```output2
Possible
7 5 2 1 6 8 3 4 9
```




```output3
Impossible

```



## Note

<p>In the first sample from the statement the order of events could be as follows: </p><ul> <li> student 4 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">4</sub> = 0</span>), he has no one to greet; </li><li> student 5 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">5</sub> = 1</span>), he shakes hands with student 4; </li><li> student 1 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 2</span>), he shakes hands with two students (students 4, 5); </li><li> student 3 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = 3</span>), he shakes hands with three students (students 4, 5, 1); </li><li> students 4, 5, 3 form a team and start writing a contest; </li><li> student 2 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 1</span>), he shakes hands with one student (number 1). </li></ul><p>In the second sample from the statement the order of events could be as follows: </p><ul> <li> student 7 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">7</sub> = 0</span>), he has nobody to greet; </li><li> student 5 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">5</sub> = 1</span>), he shakes hands with student 7; </li><li> student 2 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 2</span>), he shakes hands with two students (students 7, 5); </li><li> students 7, 5, 2 form a team and start writing a contest; </li><li> student 1 comes in(<span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>), he has no one to greet (everyone is busy with the contest); </li><li> student 6 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">6</sub> = 1</span>), he shakes hands with student 1; </li><li> student 8 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">8</sub> = 2</span>), he shakes hands with two students (students 1, 6); </li><li> student 3 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = 3</span>), he shakes hands with three students (students 1, 6, 8); </li><li> student 4 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">4</sub> = 4</span>), he shakes hands with four students (students 1, 6, 8, 3); </li><li> students 8, 3, 4 form a team and start writing a contest; </li><li> student 9 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">9</sub> = 2</span>), he shakes hands with two students (students 1, 6). </li></ul><p>In the third sample from the statement the order of events is restored unambiguously: </p><ul> <li> student 1 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>), he has no one to greet; </li><li> student 3 comes in (or student 4) (<span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = <i>a</i><sub class="lower-index">4</sub> = 1</span>), he shakes hands with student 1; </li><li> student 2 comes in (<span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 2</span>), he shakes hands with two students (students 1, 3 (or 4)); </li><li> the remaining student 4 (or student 3), must shake one student's hand (<span class="tex-span"><i>a</i><sub class="lower-index">3</sub> = <i>a</i><sub class="lower-index">4</sub> = 1</span>) but it is impossible as there are only two scenarios: either a team formed and he doesn't greet anyone, or he greets all the three present people who work individually. </li></ul>
