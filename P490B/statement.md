## Description

<div><p>During the lunch break all <span class="tex-span"><i>n</i></span> Berland State University students lined up in the food court. However, it turned out that the food court, too, has a lunch break and it temporarily stopped working.</p><p>Standing in a queue that isn't being served is so boring! So, each of the students wrote down the number of the student ID of the student that stands in line directly in front of him, and the student that stands in line directly behind him. If no one stands before or after a student (that is, he is the first one or the last one), then he writes down number <span class="tex-font-style-tt">0</span> instead (in Berland State University student IDs are numerated from <span class="tex-span">1</span>).</p><p>After that, all the students went about their business. When they returned, they found out that restoring the queue is not such an easy task.</p><p>Help the students to restore the state of the queue by the numbers of the student ID's of their neighbors in the queue.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of students in the queue. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line contains the pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the ID number of a person in front of a student and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the ID number of a person behind a student. The lines are given in the arbitrary order. Value <span class="tex-font-style-tt">0</span> is given instead of a neighbor's ID number if the neighbor doesn't exist.</p><p>The ID numbers of all students are distinct. It is guaranteed that the records correspond too the queue where all the students stand in some order.</p></div><div class="output-specification"><p>Print a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> — the sequence of ID numbers of all the students in the order they go in the queue from the first student to the last one.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of students in the queue. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line contains the pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the ID number of a person in front of a student and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the ID number of a person behind a student. The lines are given in the arbitrary order. Value <span class="tex-font-style-tt">0</span> is given instead of a neighbor's ID number if the neighbor doesn't exist.</p><p>The ID numbers of all students are distinct. It is guaranteed that the records correspond too the queue where all the students stand in some order.</p>

## Output

<p>Print a sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> — the sequence of ID numbers of all the students in the order they go in the queue from the first student to the last one.</p>





```input1
4
92 31
0 7
31 0
7 141

```




```output1
92 7 31 141 

```



## Note

<p>The picture illustrates the queue for the first sample.</p><center> <img class="tex-graphics" src="file://9FL8MiCK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
