## Description

<div><p>Of course our child likes walking in a zoo. The zoo has <span class="tex-span"><i>n</i></span> areas, that are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th area contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> animals in it. Also there are <span class="tex-span"><i>m</i></span> roads in the zoo, and each road connects two distinct areas. Naturally the zoo is connected, so you can reach any area of the zoo from any other area using the roads.</p><p>Our child is very smart. Imagine the child want to go from area <span class="tex-span"><i>p</i></span> to area <span class="tex-span"><i>q</i></span>. Firstly he considers all the simple routes from <span class="tex-span"><i>p</i></span> to <span class="tex-span"><i>q</i></span>. For each route the child writes down the number, that is equal to the minimum number of animals among the route areas. Let's denote the largest of the written numbers as <span class="tex-span"><i>f</i>(<i>p</i>, <i>q</i>)</span>. Finally, the child chooses one of the routes for which he writes down the value <span class="tex-span"><i>f</i>(<i>p</i>, <i>q</i>)</span>.</p><p>After the child has visited the zoo, he thinks about the question: what is the average value of <span class="tex-span"><i>f</i>(<i>p</i>, <i>q</i>)</span> for all pairs <span class="tex-span"><i>p</i>, <i>q</i></span> <span class="tex-span">(<i>p</i> ≠ <i>q</i>)</span>? Can you answer his question?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). Then follow <span class="tex-span"><i>m</i></span> lines, each line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), denoting the road between areas <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>All roads are bidirectional, each pair of areas is connected by at most one road.</p></div><div class="output-specification"><p>Output a real number — the value of <img align="middle" class="tex-formula" src="file://kj19iwlg.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>; <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). Then follow <span class="tex-span"><i>m</i></span> lines, each line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), denoting the road between areas <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>All roads are bidirectional, each pair of areas is connected by at most one road.</p>

## Output

<p>Output a real number — the value of <img align="middle" class="tex-formula" src="file://kj19iwlg.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
4 3
10 20 30 40
1 3
2 3
4 3

```




```input2
3 3
10 20 30
1 2
2 3
3 1

```




```input3
7 8
40 20 10 30 20 50 40
1 2
2 3
3 4
4 5
5 6
6 7
1 4
5 7

```




```output1
16.666667

```




```output2
13.333333

```




```output3
18.571429

```



## Note

<p>Consider the first sample. There are <span class="tex-span">12</span> possible situations:</p><ul> <li> <span class="tex-span"><i>p</i> = 1, <i>q</i> = 3, <i>f</i>(<i>p</i>, <i>q</i>) = 10</span>. </li><li> <span class="tex-span"><i>p</i> = 2, <i>q</i> = 3, <i>f</i>(<i>p</i>, <i>q</i>) = 20</span>. </li><li> <span class="tex-span"><i>p</i> = 4, <i>q</i> = 3, <i>f</i>(<i>p</i>, <i>q</i>) = 30</span>. </li><li> <span class="tex-span"><i>p</i> = 1, <i>q</i> = 2, <i>f</i>(<i>p</i>, <i>q</i>) = 10</span>. </li><li> <span class="tex-span"><i>p</i> = 2, <i>q</i> = 4, <i>f</i>(<i>p</i>, <i>q</i>) = 20</span>. </li><li> <span class="tex-span"><i>p</i> = 4, <i>q</i> = 1, <i>f</i>(<i>p</i>, <i>q</i>) = 10</span>. </li></ul><p>Another <span class="tex-span">6</span> cases are symmetrical to the above. The average is <img align="middle" class="tex-formula" src="file://kiWJWiOd.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Consider the second sample. There are <span class="tex-span">6</span> possible situations:</p><ul> <li> <span class="tex-span"><i>p</i> = 1, <i>q</i> = 2, <i>f</i>(<i>p</i>, <i>q</i>) = 10</span>. </li><li> <span class="tex-span"><i>p</i> = 2, <i>q</i> = 3, <i>f</i>(<i>p</i>, <i>q</i>) = 20</span>. </li><li> <span class="tex-span"><i>p</i> = 1, <i>q</i> = 3, <i>f</i>(<i>p</i>, <i>q</i>) = 10</span>. </li></ul><p>Another <span class="tex-span">3</span> cases are symmetrical to the above. The average is <img align="middle" class="tex-formula" src="file://aanaeZZ9.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
