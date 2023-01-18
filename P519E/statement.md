## Description

<div><p><span class="tex-font-style-it">A and B are preparing themselves for programming contests.</span></p><p>The University where A and B study is a set of rooms connected by corridors. Overall, the University has <span class="tex-span"><i>n</i></span> rooms connected by <span class="tex-span"><i>n</i> - 1</span> corridors so that you can get from any room to any other one by moving along the corridors. The rooms are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Every day А and B write contests in some rooms of their university, and after each contest they gather together in the same room and discuss problems. A and B want the distance from the rooms where problems are discussed to the rooms where contests are written to be equal. The distance between two rooms is the number of edges on the shortest path between them.</p><p>As they write contests in new rooms every day, they asked you to help them find the number of possible rooms to discuss problems for each of the following <span class="tex-span"><i>m</i></span> days.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of rooms in the University.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines describe the corridors. The <span class="tex-span"><i>i</i></span>-th of these lines (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), showing that the <span class="tex-span"><i>i</i></span>-th corridor connects rooms <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the queries. The <span class="tex-span"><i>j</i></span>-th of these lines (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) that means that on the <span class="tex-span"><i>j</i></span>-th day A will write the contest in the room <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, B will write in the room <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>In the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) line print the number of rooms that are equidistant from the rooms where A and B write contest on the <span class="tex-span"><i>i</i></span>-th day.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of rooms in the University.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines describe the corridors. The <span class="tex-span"><i>i</i></span>-th of these lines (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), showing that the <span class="tex-span"><i>i</i></span>-th corridor connects rooms <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the queries. The <span class="tex-span"><i>j</i></span>-th of these lines (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>j</i></sub>, <i>y</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) that means that on the <span class="tex-span"><i>j</i></span>-th day A will write the contest in the room <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span>, B will write in the room <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub></span>.</p>

## Output

<p>In the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>) line print the number of rooms that are equidistant from the rooms where A and B write contest on the <span class="tex-span"><i>i</i></span>-th day.</p>





```input1
4
1 2
1 3
2 4
1
2 3

```




```input2
4
1 2
2 3
2 4
2
1 2
1 3

```




```output1
1

```




```output2
0
2

```



## Note

<p>in the first sample there is only one room at the same distance from rooms number 2 and 3 — room number 1.</p>
