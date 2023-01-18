## Description

<div><p>Many students live in a dormitory. A dormitory is a whole new world of funny amusements and possibilities but it does have its drawbacks. </p><p>There is only one shower and there are multiple students who wish to have a shower in the morning. That's why every morning there is a line of five people in front of the dormitory shower door. As soon as the shower opens, the first person from the line enters the shower. After a while the first person leaves the shower and the next person enters the shower. The process continues until everybody in the line has a shower.</p><p>Having a shower takes some time, so the students in the line talk as they wait. At each moment of time the students talk in pairs: the <span class="tex-span">(2<i>i</i> - 1)</span>-th man in the line (for the current moment) talks with the <span class="tex-span">(2<i>i</i>)</span>-th one. </p><p>Let's look at this process in more detail. Let's number the people from 1 to 5. Let's assume that the line initially looks as 23154 (person number 2 stands at the beginning of the line). Then, before the shower opens, 2 talks with 3, 1 talks with 5, 4 doesn't talk with anyone. Then 2 enters the shower. While 2 has a shower, 3 and 1 talk, 5 and 4 talk too. Then, 3 enters the shower. While 3 has a shower, 1 and 5 talk, 4 doesn't talk to anyone. Then 1 enters the shower and while he is there, 5 and 4 talk. Then 5 enters the shower, and then 4 enters the shower.</p><p>We know that if students <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> talk, then the <span class="tex-span"><i>i</i></span>-th student's happiness increases by <span class="tex-span"><i>g</i><sub class="lower-index"><i>ij</i></sub></span> and the <span class="tex-span"><i>j</i></span>-th student's happiness increases by <span class="tex-span"><i>g</i><sub class="lower-index"><i>ji</i></sub></span>. Your task is to find such initial order of students in the line that the total happiness of all students will be maximum in the end. Please note that some pair of students may have a talk several times. In the example above students 1 and 5 talk while they wait for the shower to open and while 3 has a shower.</p></div><div class="input-specification"><p>The input consists of five lines, each line contains five space-separated integers: the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line shows <span class="tex-span"><i>g</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>g</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). It is guaranteed that <span class="tex-span"><i>g</i><sub class="lower-index"><i>ii</i></sub> = 0</span> for all <span class="tex-span"><i>i</i></span>.</p><p>Assume that the students are numbered from 1 to 5.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible total happiness of the students.</p></div>

## Input

<p>The input consists of five lines, each line contains five space-separated integers: the <span class="tex-span"><i>j</i></span>-th number in the <span class="tex-span"><i>i</i></span>-th line shows <span class="tex-span"><i>g</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">0 ≤ <i>g</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). It is guaranteed that <span class="tex-span"><i>g</i><sub class="lower-index"><i>ii</i></sub> = 0</span> for all <span class="tex-span"><i>i</i></span>.</p><p>Assume that the students are numbered from 1 to 5.</p>

## Output

<p>Print a single integer — the maximum possible total happiness of the students.</p>





```input1
0 0 0 0 9
0 0 0 0 0
0 0 0 0 0
0 0 0 0 0
7 0 0 0 0

```




```input2
0 43 21 18 2
3 0 21 11 65
5 2 0 1 4
54 62 12 0 99
87 64 81 33 0

```




```output1
32

```




```output2
620

```



## Note

<p>In the first sample, the optimal arrangement of the line is 23154. In this case, the total happiness equals:</p><center class="tex-equation"><span class="tex-span">(<i>g</i><sub class="lower-index">23</sub> + <i>g</i><sub class="lower-index">32</sub> + <i>g</i><sub class="lower-index">15</sub> + <i>g</i><sub class="lower-index">51</sub>) + (<i>g</i><sub class="lower-index">13</sub> + <i>g</i><sub class="lower-index">31</sub> + <i>g</i><sub class="lower-index">54</sub> + <i>g</i><sub class="lower-index">45</sub>) + (<i>g</i><sub class="lower-index">15</sub> + <i>g</i><sub class="lower-index">51</sub>) + (<i>g</i><sub class="lower-index">54</sub> + <i>g</i><sub class="lower-index">45</sub>) = 32</span></center>.
