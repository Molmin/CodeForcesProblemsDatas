## Description

<div><p>Berlanders like to eat cones after a hard day. Misha Square and Sasha Circle are local authorities of Berland. Each of them controls its points of cone trade. Misha has <span class="tex-span"><i>n</i></span> points, Sasha — <span class="tex-span"><i>m</i></span>. Since their subordinates constantly had conflicts with each other, they decided to build a fence in the form of a circle, so that the points of trade of one businessman are strictly inside a circle, and points of the other one are strictly outside. It doesn't matter which of the two gentlemen will have his trade points inside the circle.</p><p>Determine whether they can build a fence or not.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10000)</span>, numbers of Misha's and Sasha's trade points respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains pairs of space-separated integers <span class="tex-span"><i>M</i><sub class="lower-index"><i>x</i></sub>, <i>M</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>M</i><sub class="lower-index"><i>x</i></sub>, <i>M</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), coordinates of Misha's trade points.</p><p>The next <span class="tex-span"><i>m</i></span> lines contains pairs of space-separated integers <span class="tex-span"><i>S</i><sub class="lower-index"><i>x</i></sub>, <i>S</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>S</i><sub class="lower-index"><i>x</i></sub>, <i>S</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), coordinates of Sasha's trade points.</p><p>It is guaranteed that all <span class="tex-span"><i>n</i> + <i>m</i></span> points are distinct.</p></div><div class="output-specification"><p>The only output line should contain either word "<span class="tex-font-style-tt">YES</span>" without quotes in case it is possible to build a such fence or word "<span class="tex-font-style-tt">NO</span>" in the other case.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10000)</span>, numbers of Misha's and Sasha's trade points respectively.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains pairs of space-separated integers <span class="tex-span"><i>M</i><sub class="lower-index"><i>x</i></sub>, <i>M</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>M</i><sub class="lower-index"><i>x</i></sub>, <i>M</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), coordinates of Misha's trade points.</p><p>The next <span class="tex-span"><i>m</i></span> lines contains pairs of space-separated integers <span class="tex-span"><i>S</i><sub class="lower-index"><i>x</i></sub>, <i>S</i><sub class="lower-index"><i>y</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>S</i><sub class="lower-index"><i>x</i></sub>, <i>S</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), coordinates of Sasha's trade points.</p><p>It is guaranteed that all <span class="tex-span"><i>n</i> + <i>m</i></span> points are distinct.</p>

## Output

<p>The only output line should contain either word "<span class="tex-font-style-tt">YES</span>" without quotes in case it is possible to build a such fence or word "<span class="tex-font-style-tt">NO</span>" in the other case.</p>





```input1
2 2
-1 0
1 0
0 -1
0 1

```




```input2
4 4
1 0
0 1
-1 0
0 -1
1 1
-1 1
-1 -1
1 -1

```




```output1
NO

```




```output2
YES

```



## Note

<p>In the first sample there is no possibility to separate points, because any circle that contains both points <span class="tex-span">( - 1, 0), (1, 0)</span> also contains at least one point from the set <span class="tex-span">(0,  - 1), (0, 1)</span>, and vice-versa: any circle that contains both points <span class="tex-span">(0,  - 1), (0, 1)</span> also contains at least one point from the set <span class="tex-span">( - 1, 0), (1, 0)</span></p><p>In the second sample one of the possible solution is shown below. Misha's points are marked with red colour and Sasha's are marked with blue. <img class="tex-graphics" src="file://I1UjloPX.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
