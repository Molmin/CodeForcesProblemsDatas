## Description

<div><p>Students of group 199 have written their lectures dismally. Now an exam on Mathematical Analysis is approaching and something has to be done asap (that is, quickly). Let's number the students of the group from 1 to <span class="tex-span"><i>n</i></span>. Each student <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) has a best friend <span class="tex-span"><i>p</i>[<i>i</i>]</span> (<span class="tex-span">1 ≤ <i>p</i>[<i>i</i>] ≤ <i>n</i></span>). In fact, each student is a best friend of <span class="tex-font-style-it">exactly one</span> student. In other words, all <span class="tex-span"><i>p</i>[<i>i</i>]</span> are different. It is possible that the group also has some really "special individuals" for who <span class="tex-span"><i>i</i> = <i>p</i>[<i>i</i>]</span>.</p><p>Each student wrote exactly one notebook of lecture notes. We know that the students agreed to act by the following algorithm: </p><ul> <li> on the first day of revising each student studies his own Mathematical Analysis notes, </li><li> in the morning of each following day each student gives the notebook to his best friend and takes a notebook from the student who calls him the best friend. </li></ul><p>Thus, on the second day the student <span class="tex-span"><i>p</i>[<i>i</i>]</span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) studies the <span class="tex-span"><i>i</i></span>-th student's notes, on the third day the notes go to student <span class="tex-span"><i>p</i>[<i>p</i>[<i>i</i>]]</span> and so on. Due to some characteristics of the boys' friendship (see paragraph 1), each day each student has exactly one notebook to study.</p><p>You are given two sequences that describe the situation on the third and fourth days of revising:</p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means the student who gets the <span class="tex-span"><i>i</i></span>-th student's notebook on the third day of revising; </li><li> <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> means the student who gets the <span class="tex-span"><i>i</i></span>-th student's notebook on the fourth day of revising. </li></ul><p>You do not know array <span class="tex-span"><i>p</i></span>, that is you do not know who is the best friend to who. Write a program that finds <span class="tex-span"><i>p</i></span> by the given sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of students in the group. The second line contains sequence of different integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). The third line contains the sequence of different integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print sequence <span class="tex-span"><i>n</i></span> of different integers <span class="tex-span"><i>p</i>[1], <i>p</i>[2], ..., <i>p</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>p</i>[<i>i</i>] ≤ <i>n</i></span>). It is guaranteed that the solution exists and that it is unique.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of students in the group. The second line contains sequence of different integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). The third line contains the sequence of different integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print sequence <span class="tex-span"><i>n</i></span> of different integers <span class="tex-span"><i>p</i>[1], <i>p</i>[2], ..., <i>p</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>p</i>[<i>i</i>] ≤ <i>n</i></span>). It is guaranteed that the solution exists and that it is unique.</p>





```input1
4
2 1 4 3
3 4 2 1

```




```input2
5
5 2 3 1 4
1 3 2 4 5

```




```input3
2
1 2
2 1

```




```output1
4 3 1 2
```




```output2
4 3 2 5 1
```




```output3
2 1
```


