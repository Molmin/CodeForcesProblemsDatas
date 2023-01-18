## Description

<div><p>New Year is coming in Tree Island! In this island, as the name implies, there are <span class="tex-span"><i>n</i></span> cities connected by <span class="tex-span"><i>n</i> - 1</span> roads, and for any two distinct cities there always exists exactly one path between them. For every person in Tree Island, it takes exactly one minute to pass by exactly one road.</p><p>There is a weird New Year tradition for runnners in Tree Island, which is called "extreme run". This tradition can be done as follows.</p><p>A runner chooses two distinct cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. For simplicity, let's denote the shortest path from city <span class="tex-span"><i>a</i></span> to city <span class="tex-span"><i>b</i></span> as <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>l</i></sub></span> (here, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = <i>a</i></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>l</i></sub> = <i>b</i></span> holds). Then following happens:</p><ol> <li> The runner starts at city <span class="tex-span"><i>a</i></span>. </li><li> The runner runs from city <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>, following the shortest path from city <span class="tex-span"><i>a</i></span> to city <span class="tex-span"><i>b</i></span>. </li><li> When the runner arrives at city <span class="tex-span"><i>b</i></span>, he turns his direction immediately (it takes no time), and runs towards city <span class="tex-span"><i>a</i></span>, following the shortest path from city <span class="tex-span"><i>b</i></span> to city <span class="tex-span"><i>a</i></span>. </li><li> When the runner arrives at city <span class="tex-span"><i>a</i></span>, he turns his direction immediately (it takes no time), and runs towards city <span class="tex-span"><i>b</i></span>, following the shortest path from city <span class="tex-span"><i>a</i></span> to city <span class="tex-span"><i>b</i></span>. </li><li> Repeat step 3 and step 4 forever. </li></ol><p>In short, the course of the runner can be denoted as: <img align="middle" class="tex-formula" src="file://nIoPiagw.png" style="max-width: 100.0%;max-height: 100.0%;"> <img align="middle" class="tex-formula" src="file://TZwnGcB5.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Two runners JH and JY decided to run "extremely" in order to celebrate the New Year. JH has chosen two cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, and JY has chosen two cities <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. They decided to start running at the same moment, and run until they meet at the same city for the first time. Meeting on a road doesn't matter for them. Before running, they want to know the amount of time they will run.</p><p>It is too hard for JH and JY to calculate this, so they ask you for help.</p></div><div class="input-specification"><p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>) — the number of cities in Tree Island.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the roads of Tree Island. The <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the vertices connected by a single road of the tree.</p><p>The next line contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>) — the number of test cases.</p><p>Next <span class="tex-span"><i>t</i></span> lines describes the test cases. The <span class="tex-span"><i>j</i></span>-th line (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>t</i></span>) of them contains four space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>x</i><sub class="lower-index"><i>j</i></sub> ≠ <i>y</i><sub class="lower-index"><i>j</i></sub></span>). It means that in this test case, JH has chosen two cities <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span>, JY has chosen two cities <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>. JH starts running at city <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span>, and JY starts running at city <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>For each test case, print an integer describing the amount of time they should run in minutes. If they have to run for an infinitely long time (in other words, if they never meet at the same city), print -1 instead. If they meet at the beginning of their run, print 0.</p></div>

## Input

<p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>) — the number of cities in Tree Island.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the roads of Tree Island. The <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the vertices connected by a single road of the tree.</p><p>The next line contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>) — the number of test cases.</p><p>Next <span class="tex-span"><i>t</i></span> lines describes the test cases. The <span class="tex-span"><i>j</i></span>-th line (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>t</i></span>) of them contains four space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub>, <i>x</i><sub class="lower-index"><i>j</i></sub> ≠ <i>y</i><sub class="lower-index"><i>j</i></sub></span>). It means that in this test case, JH has chosen two cities <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span>, JY has chosen two cities <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>. JH starts running at city <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span>, and JY starts running at city <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>.</p>

## Output

<p>For each test case, print an integer describing the amount of time they should run in minutes. If they have to run for an infinitely long time (in other words, if they never meet at the same city), print -1 instead. If they meet at the beginning of their run, print 0.</p>





```input1
7
1 3
3 6
7 4
3 7
5 4
7 2
4
6 5 5 3
3 5 4 6
1 5 1 3
1 5 3 1

```




```output1
2
1
0
-1

```



## Note

<p>The example looks like:</p><center> <img class="tex-graphics" src="file://HuFWGdlC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
