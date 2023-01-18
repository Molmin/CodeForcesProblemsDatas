## Description

<div><p>Robot Bender decided to make Fray a birthday present. He drove <span class="tex-span"><i>n</i></span> nails and numbered them from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in some order. Bender decided to make a picture using metal rods. The picture is a closed polyline, which vertices should be nails (in the given order). The segments of the polyline should be parallel to the coordinate axes. Polyline is allowed to have self-intersections. Bender can take a rod and fold it exactly once in any place to form an angle of 90 degrees. Then he can attach the place of the fold to some unoccupied nail and attach two ends of this rod to adjacent nails. A nail is considered unoccupied if there is no rod attached to it (neither by it's end nor the by the fold place). No rod could be used twice. It is not required to use all the rods.</p><p>Help Bender to solve this difficult task.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 500, 2 ≤ <i>m</i> ≤ 500</span>, <span class="tex-span"><i>n</i></span> is even) — the amount of nails and the amount of rods. <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains a pair of integers, denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th nail. Nails should be connected in the same order as they are given in the input. The last line contains <span class="tex-span"><i>m</i></span> integers — the lenghts of the rods. All coordinates do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> by absolute value. Lengths of the rods are between <span class="tex-span">1</span> and <span class="tex-span">200 000</span>. No rod can be used twice. It is guaranteed that all segments of the given polyline are parallel to coordinate axes. No three consecutive nails lie on the same line.</p></div><div class="output-specification"><p>If it is impossible to solve Bender's problem, output <span class="tex-font-style-tt">NO</span>. Otherwise, output <span class="tex-font-style-tt">YES</span> in the first line, and in the second line output <span class="tex-span"><i>n</i></span> numbers — <span class="tex-span"><i>i</i></span>-th of them should be the number of rod, which fold place is attached to the <span class="tex-span"><i>i</i></span>-th nail, or <span class="tex-font-style-tt">-1</span>, if there is no such rod.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 500, 2 ≤ <i>m</i> ≤ 500</span>, <span class="tex-span"><i>n</i></span> is even) — the amount of nails and the amount of rods. <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains a pair of integers, denoting the coordinates of the <span class="tex-span"><i>i</i></span>-th nail. Nails should be connected in the same order as they are given in the input. The last line contains <span class="tex-span"><i>m</i></span> integers — the lenghts of the rods. All coordinates do not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> by absolute value. Lengths of the rods are between <span class="tex-span">1</span> and <span class="tex-span">200 000</span>. No rod can be used twice. It is guaranteed that all segments of the given polyline are parallel to coordinate axes. No three consecutive nails lie on the same line.</p>

## Output

<p>If it is impossible to solve Bender's problem, output <span class="tex-font-style-tt">NO</span>. Otherwise, output <span class="tex-font-style-tt">YES</span> in the first line, and in the second line output <span class="tex-span"><i>n</i></span> numbers — <span class="tex-span"><i>i</i></span>-th of them should be the number of rod, which fold place is attached to the <span class="tex-span"><i>i</i></span>-th nail, or <span class="tex-font-style-tt">-1</span>, if there is no such rod.</p><p>If there are multiple solutions, print any of them.</p>





```input1
4 2
0 0
0 2
2 2
2 0
4 4

```




```input2
6 3
0 0
1 0
1 1
2 1
2 2
0 2
3 2 3

```




```input3
6 3
0 0
1 0
1 1
2 1
2 2
0 2
2 2 3

```




```output1
YES
1 -1 2 -1 

```




```output2
YES
1 -1 2 -1 3 -1 

```




```output3
NO

```


