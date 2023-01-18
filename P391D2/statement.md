## Description

<div><p><span class="tex-font-style-it">This problem consists of two subproblems: for solving subproblem D1 you will receive 3 points, and for solving subproblem D2 you will receive 16 points.</span></p><p>Manao is the chief architect involved in planning a new supercollider. He has to identify a plot of land where the largest possible supercollider can be built. The supercollider he is building requires four-way orthogonal collisions of particles traveling at the same speed, so it will consist of four accelerating chambers and be shaped like a plus sign (i.e., +). Each of the four accelerating chambers must be the same length and must be aligned with the Earth's magnetic field (parallel or orthogonal) to minimize interference.</p><p>The accelerating chambers need to be laid down across long flat stretches of land to keep costs under control. Thus, Manao has already commissioned a topographical study that has identified all possible maximal length tracts of land available for building accelerating chambers that are either parallel or orthogonal to the Earth's magnetic field. To build the largest possible supercollider, Manao must identify the largest symmetric plus shape from among these candidate tracts. That is, he must find the two tracts of land that form an axis-aligned plus shape with the largest distance from the center of the plus to the tip of the shortest of the four arms of the plus. Note that the collider need not use the entire length of the tracts identified (see the example in the notes).</p></div><div class="input-specification"><p>The first line of the input will contain two single-space-separated integers <span class="tex-span"><i>n</i></span>, the number of north-south tracts and <span class="tex-span"><i>m</i></span>, the number of west-east tracts.</p><p>Each of the <span class="tex-span"><i>n</i></span> lines following the first describes a north-south tract. Each such tract is described by three single-space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> representing the vertical line segment from <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> + <i>l</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>Similarly, after the <span class="tex-span"><i>n</i></span> lines describing north-south tracts follow <span class="tex-span"><i>m</i></span> similar lines describing the west-east tracts. Each such tract is described by three single-space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> representing the horizontal line segment from <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> + <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are between -100000000 and 100000000, inclusive. All <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> are between 1 and 100000000, inclusive. No pair of horizontal segments will touch or intersect, and no pair of vertical segments will touch or intersect.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem D1 (3 points), <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">1000</span>, inclusive. </li><li> In subproblem D2 (16 points), <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">50000</span>, inclusive. </li></ul></div><div class="output-specification"><p>Print one line containing a single integer, the size of the largest supercollider that can be built on one north-south tract and one west-east tract. The size of the supercollider is defined to be the length of one of the four accelerating chambers. In other words, the size of the resulting supercollider is defined to be the distance from the intersection of the two line segments to the closest endpoint of either of the two segments. If no pair of north-south and west-east tracts intersects, it is not possible to build a supercollider and the program should report a maximum size of zero.</p></div>

## Input

<p>The first line of the input will contain two single-space-separated integers <span class="tex-span"><i>n</i></span>, the number of north-south tracts and <span class="tex-span"><i>m</i></span>, the number of west-east tracts.</p><p>Each of the <span class="tex-span"><i>n</i></span> lines following the first describes a north-south tract. Each such tract is described by three single-space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> representing the vertical line segment from <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> + <i>l</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>Similarly, after the <span class="tex-span"><i>n</i></span> lines describing north-south tracts follow <span class="tex-span"><i>m</i></span> similar lines describing the west-east tracts. Each such tract is described by three single-space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> representing the horizontal line segment from <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> to <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> + <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are between -100000000 and 100000000, inclusive. All <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> are between 1 and 100000000, inclusive. No pair of horizontal segments will touch or intersect, and no pair of vertical segments will touch or intersect.</p><p><span class="tex-font-style-it">The problem consists of two subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem D1 (3 points), <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">1000</span>, inclusive. </li><li> In subproblem D2 (16 points), <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> will be between <span class="tex-span">1</span> and <span class="tex-span">50000</span>, inclusive. </li></ul>

## Output

<p>Print one line containing a single integer, the size of the largest supercollider that can be built on one north-south tract and one west-east tract. The size of the supercollider is defined to be the length of one of the four accelerating chambers. In other words, the size of the resulting supercollider is defined to be the distance from the intersection of the two line segments to the closest endpoint of either of the two segments. If no pair of north-south and west-east tracts intersects, it is not possible to build a supercollider and the program should report a maximum size of zero.</p>





```input1
1 2
4 0 9
1 1 8
1 2 7

```




```output1
2

```



## Note

<p>Consider the example. There is one vertical line segment from (4, 0) to (4, 9) and two horizontal line segments: from (1, 1) to (9, 1) and from (1, 2) to (8, 2). The largest plus shape that can be found among these segments is formed from the only vertical segment and the second of horizontal segments, and is centered at (4, 2). </p><p>The program should output 2 because the closest end point of those segments to the center is (4, 0), which is distance 2 from the center point of (4, 2). The collider will be formed by the line segments from (2, 2) to (6, 2) and from (4, 0) to (4, 4).</p>