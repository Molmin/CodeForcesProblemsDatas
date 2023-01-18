## Description

<div><p>There is a bus stop near the university. The lessons are over, and <span class="tex-span"><i>n</i></span> students come to the stop. The <span class="tex-span"><i>i</i></span>-th student will appear at the bus stop at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>'s are distinct).</p><p>We shall assume that the stop is located on the coordinate axis <span class="tex-span"><i>Ox</i></span>, at point <span class="tex-span"><i>x</i> = 0</span>, and the bus goes along the ray <span class="tex-span"><i>Ox</i></span>, that is, towards the positive direction of the coordinate axis, and back. The <span class="tex-span"><i>i</i></span>-th student needs to get to the point with coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span>).</p><p>The bus moves by the following algorithm. Initially it is at point 0. The students consistently come to the stop and get on it. The bus has a seating capacity which is equal to <span class="tex-span"><i>m</i></span> passengers. At the moment when <span class="tex-span"><i>m</i></span> students get on the bus, it starts moving in the positive direction of the coordinate axis. Also it starts moving when the last (<span class="tex-span"><i>n</i></span>-th) student gets on the bus. The bus is moving at a speed of 1 unit of distance per 1 unit of time, i.e. it covers distance <span class="tex-span"><i>y</i></span> in time <span class="tex-span"><i>y</i></span>.</p><p>Every time the bus passes the point at which at least one student needs to get off, it stops and these students get off the bus. The students need <span class="tex-span">1 + [<i>k</i> / 2]</span> units of time to get off the bus, where <span class="tex-span"><i>k</i></span> is the number of students who leave at this point. Expression <span class="tex-span">[<i>k</i> / 2]</span> denotes rounded down <span class="tex-span"><i>k</i> / 2</span>. As soon as the last student leaves the bus, the bus turns around and goes back to the point <span class="tex-span"><i>x</i> = 0</span>. It doesn't make any stops until it reaches the point. At the given point the bus fills with students once more, and everything is repeated.</p><p>If students come to the stop when there's no bus, they form a line (queue) and get on the bus in the order in which they came. Any number of students get on the bus in negligible time, you should assume that it doesn't take any time. Any other actions also take no time. The bus has no other passengers apart from the students.</p><p>Write a program that will determine for each student the time when he got off the bus. The moment a student got off the bus is the moment the bus stopped at the student's destination stop (despite the fact that the group of students need some time to get off).</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of students and the number of passengers the bus can transport, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain descriptions of the students, one per line. Each line contains a pair of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). The lines are given in the order of strict increasing of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Values of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> can coincide.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> — the moment of time when the <span class="tex-span"><i>i</i></span>-th student got off the bus. Print the numbers on one line and separate them with single spaces.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of students and the number of passengers the bus can transport, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain descriptions of the students, one per line. Each line contains a pair of integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). The lines are given in the order of strict increasing of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. Values of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> can coincide.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> — the moment of time when the <span class="tex-span"><i>i</i></span>-th student got off the bus. Print the numbers on one line and separate them with single spaces.</p>





```input1
1 10
3 5

```




```input2
2 1
3 5
4 5

```




```input3
5 4
3 5
4 5
5 5
6 5
7 1

```




```input4
20 4
28 13
31 13
35 6
36 4
52 6
53 4
83 2
84 4
87 1
93 6
108 4
113 6
116 1
125 2
130 2
136 13
162 2
166 4
184 1
192 2

```




```output1
8

```




```output2
8 19

```




```output3
11 11 11 11 20

```




```output4
51 51 43 40 93 89 86 89 114 121 118 121 137 139 139 152 195 199 193 195

```



## Note

<p>In the first sample the bus waits for the first student for <span class="tex-span">3</span> units of time and drives him to his destination in additional <span class="tex-span">5</span> units of time. So the student leaves the bus at the moment of time <span class="tex-span">3 + 5 = 8</span>.</p><p>In the second sample the capacity of the bus equals <span class="tex-span">1</span>, that's why it will drive the first student alone. This student is the same as the student from the first sample. So the bus arrives to his destination at the moment of time <span class="tex-span">8</span>, spends <span class="tex-span">1 + [1 / 2] = 1</span> units of time on getting him off, and returns back to <span class="tex-span">0</span> in additional <span class="tex-span">5</span> units of time. That is, the bus returns to the bus stop at the moment of time <span class="tex-span">14</span>. By this moment the second student has already came to the bus stop. So he immediately gets in the bus, and is driven to his destination in additional <span class="tex-span">5</span> units of time. He gets there at the moment <span class="tex-span">14 + 5 = 19</span>. </p><p>In the third sample the bus waits for the fourth student for <span class="tex-span">6</span> units of time, then drives for <span class="tex-span">5</span> units of time, then gets the passengers off for <span class="tex-span">1 + [4 / 2] = 3</span> units of time, then returns for <span class="tex-span">5</span> units of time, and then drives the fifth student for <span class="tex-span">1</span> unit of time.</p>
