## Description

<div><p>Anna and Maria are in charge of the math club for junior students. When the club gathers together, the students behave badly. They've brought lots of shoe laces to the club and got tied with each other. Specifically, each string ties together two students. Besides, if two students are tied, then the lace connects the first student with the second one as well as the second student with the first one.</p><p>To restore order, Anna and Maria do the following. First, for each student Anna finds out what other students he is tied to. If a student is tied to exactly one other student, Anna reprimands him. Then Maria gathers in a single group <span class="tex-font-style-bf">all</span> the students who have been just reprimanded. She kicks them out from the club. This group of students immediately leaves the club. These students takes with them the laces that used to tie them. Then again for every student Anna finds out how many other students he is tied to and so on. And they do so until Anna can reprimand at least one student.</p><p>Determine how many groups of students will be kicked out of the club.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the initial number of students and laces (<img align="middle" class="tex-formula" src="file://dQpYZgFU.png" style="max-width: 100.0%;max-height: 100.0%;">). The students are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the laces are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Next <span class="tex-span"><i>m</i></span> lines each contain two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> — the numbers of students tied by the <span class="tex-span"><i>i</i></span>-th lace (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>). It is guaranteed that no two students are tied with more than one lace. No lace ties a student to himself.</p></div><div class="output-specification"><p>Print the single number — the number of groups of students that will be kicked out from the club.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the initial number of students and laces (<img align="middle" class="tex-formula" src="file://dQpYZgFU.png" style="max-width: 100.0%;max-height: 100.0%;">). The students are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the laces are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Next <span class="tex-span"><i>m</i></span> lines each contain two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> — the numbers of students tied by the <span class="tex-span"><i>i</i></span>-th lace (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>). It is guaranteed that no two students are tied with more than one lace. No lace ties a student to himself.</p>

## Output

<p>Print the single number — the number of groups of students that will be kicked out from the club.</p>





```input1
3 3
1 2
2 3
3 1

```




```input2
6 3
1 2
2 3
3 4

```




```input3
6 5
1 4
2 4
3 4
5 4
6 4

```




```output1
0

```




```output2
2

```




```output3
1

```



## Note

<p>In the first sample Anna and Maria won't kick out any group of students — in the initial position every student is tied to two other students and Anna won't be able to reprimand anyone.</p><p>In the second sample four students are tied in a chain and two more are running by themselves. First Anna and Maria kick out the two students from both ends of the chain (1 and 4), then — two other students from the chain (2 and 3). At that the students who are running by themselves will stay in the club.</p><p>In the third sample Anna and Maria will momentarily kick out all students except for the fourth one and the process stops at that point. The correct answer is one.</p>
