## Description

<div><p>The Saratov State University Olympiad Programmers Training Center (SSU OPTC) has <span class="tex-span"><i>n</i></span> students. For each student you know the number of times he/she has participated in the ACM ICPC world programming championship. According to the ACM ICPC rules, each person can participate in the world championship at most 5 times.</p><p>The head of the SSU OPTC is recently gathering teams to participate in the world championship. Each team must consist of exactly three people, at that, any person cannot be a member of two or more teams. What maximum number of teams can the head make if he wants each team to participate in the world championship with the same members at least <span class="tex-span"><i>k</i></span> times?</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000;&nbsp;1 ≤ <i>k</i> ≤ 5)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 5)</span>, where <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> shows the number of times the <span class="tex-span"><i>i</i></span>-th person participated in the ACM ICPC world championship.</p></div><div class="output-specification"><p>Print a single number — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000;&nbsp;1 ≤ <i>k</i> ≤ 5)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 5)</span>, where <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> shows the number of times the <span class="tex-span"><i>i</i></span>-th person participated in the ACM ICPC world championship.</p>

## Output

<p>Print a single number — the answer to the problem.</p>





```input1
5 2
0 4 5 1 0

```




```input2
6 4
0 1 2 3 4 5

```




```input3
6 5
0 0 0 0 0 0

```




```output1
1

```




```output2
0

```




```output3
2

```



## Note

<p>In the first sample only one team could be made: the first, the fourth and the fifth participants.</p><p>In the second sample no teams could be created.</p><p>In the third sample two teams could be created. Any partition into two teams fits.</p>
