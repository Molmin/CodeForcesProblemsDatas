## Description

<div><p>Mister B has a house in the middle of a giant plain field, which attracted aliens life. For convenience, aliens specified the Cartesian coordinate system on the field in such a way that Mister B's house has coordinates <span class="tex-span">(0, 0)</span>. After that they sent three beacons to the field, but something went wrong. One beacon was completely destroyed, while the other two landed in positions with coordinates <span class="tex-span">(<i>m</i>, 0)</span> and <span class="tex-span">(0, <i>n</i>)</span>, respectively, but shut down.</p><p>Mister B was interested in this devices, so he decided to take them home. He came to the first beacon, placed at <span class="tex-span">(<i>m</i>, 0)</span>, lifted it up and carried the beacon home choosing the shortest path. After that he came to the other beacon, placed at <span class="tex-span">(0, <i>n</i>)</span>, and also carried it home choosing the shortest path. When first beacon was lifted up, the navigation system of the beacons was activated.</p><p>Partially destroyed navigation system started to work in following way.</p><p>At time moments when both survived beacons are at points with integer coordinates the system tries to find a location for the third beacon. It succeeds if and only if there is a point with integer coordinates such that the area of the triangle formed by the two survived beacons and this point is equal to <span class="tex-span"><i>s</i></span>. In this case the system sends a packet of information with beacon positions to aliens, otherwise it doesn't.</p><p>Compute how many packets of information system sent while Mister B was moving the beacons.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>) — the number of test cases. The next <span class="tex-span">3·<i>t</i></span> lines describe <span class="tex-span"><i>t</i></span> test cases. </p><p>Every test case is described in three lines as follows. <span class="tex-font-style-bf">Note that each parameter is given as a product of three factors.</span></p><p>The first line of a test case contains three space-separated integers: <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) such that <span class="tex-span"><i>n</i> = <i>n</i><sub class="lower-index">1</sub>·<i>n</i><sub class="lower-index">2</sub>·<i>n</i><sub class="lower-index">3</sub></span>.</p><p>The second line contains three space-separated integers: <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) such that <span class="tex-span"><i>m</i> = <i>m</i><sub class="lower-index">1</sub>·<i>m</i><sub class="lower-index">2</sub>·<i>m</i><sub class="lower-index">3</sub></span>.</p><p>The third line contains three space-separated integers: <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) such that <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub>·<i>s</i><sub class="lower-index">2</sub>·<i>s</i><sub class="lower-index">3</sub></span>.</p><p><span class="tex-font-style-bf">Note that for hacks only tests with <span class="tex-span"><i>t</i> = 1</span> allowed.</span></p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> integers one per line — the answers for each test.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>) — the number of test cases. The next <span class="tex-span">3·<i>t</i></span> lines describe <span class="tex-span"><i>t</i></span> test cases. </p><p>Every test case is described in three lines as follows. <span class="tex-font-style-bf">Note that each parameter is given as a product of three factors.</span></p><p>The first line of a test case contains three space-separated integers: <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>n</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) such that <span class="tex-span"><i>n</i> = <i>n</i><sub class="lower-index">1</sub>·<i>n</i><sub class="lower-index">2</sub>·<i>n</i><sub class="lower-index">3</sub></span>.</p><p>The second line contains three space-separated integers: <span class="tex-span"><i>m</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>m</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) such that <span class="tex-span"><i>m</i> = <i>m</i><sub class="lower-index">1</sub>·<i>m</i><sub class="lower-index">2</sub>·<i>m</i><sub class="lower-index">3</sub></span>.</p><p>The third line contains three space-separated integers: <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) such that <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub>·<i>s</i><sub class="lower-index">2</sub>·<i>s</i><sub class="lower-index">3</sub></span>.</p><p><span class="tex-font-style-bf">Note that for hacks only tests with <span class="tex-span"><i>t</i> = 1</span> allowed.</span></p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> integers one per line — the answers for each test.</p>





```input1
3
2 1 1
2 1 1
1 1 3
1 5 1
2 2 1
1 1 2
10 6 18
2 103 2
13 1 13

```




```output1
4
7
171

```



## Note

<p>First test case contains the following beacon positions: <span class="tex-span">(2, 0)</span> and <span class="tex-span">(0, 2)</span>, <span class="tex-span"><i>s</i> = 3</span>. The following packets could be sent: <span class="tex-span">((2, 0), (0, 2), ( - 1, 0))</span>, <span class="tex-span">((1, 0), (0, 2), (4, 0))</span>, <span class="tex-span">((0, 0), (0, 2), (3, 1))</span>, <span class="tex-span">((0, 0), (0, 1), ( - 6, 0))</span>, where <span class="tex-span">(<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, <i>p</i>)</span> has next description: <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> — first beacon position, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> — second beacon position, <span class="tex-span"><i>p</i></span> — some generated point.</p><p>Second test case contains the following beacon initial positions: <span class="tex-span">(4, 0)</span> and <span class="tex-span">(0, 5)</span>, <span class="tex-span"><i>s</i> = 2</span>. The following packets could be sent: <span class="tex-span">((4, 0), (0, 5), (0, 4))</span>, <span class="tex-span">((3, 0), (0, 5), (2, 3))</span>, <span class="tex-span">((2, 0), (0, 5), (2, 2))</span>, <span class="tex-span">((1, 0), (0, 5), (1, 4))</span>, <span class="tex-span">((0, 0), (0, 4), (0,  - 1))</span>, <span class="tex-span">((0, 0), (0, 2), (2, 0))</span>, <span class="tex-span">((0, 0), (0, 1), (4, 0))</span>.</p>
