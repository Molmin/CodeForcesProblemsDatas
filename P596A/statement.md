## Description

<div><p>After making bad dives into swimming pools, Wilbur wants to build a swimming pool in the shape of a rectangle in his backyard. He has set up coordinate axes, and he wants the sides of the rectangle to be parallel to them. Of course, the area of the rectangle must be positive. Wilbur had all four vertices of the planned pool written on a paper, until his friend came along and erased some of the vertices.</p><p>Now Wilbur is wondering, if the remaining <span class="tex-span"><i>n</i></span> vertices of the initial rectangle give enough information to restore the area of the planned swimming pool.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4</span>)&nbsp;— the number of vertices that were <span class="tex-font-style-bf">not</span> erased by Wilbur's friend.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;—the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex that remains. Vertices are given in an arbitrary order.</p><p>It's guaranteed that these points are distinct vertices of some rectangle, that has positive area and which sides are parallel to the coordinate axes.</p></div><div class="output-specification"><p>Print the area of the initial rectangle if it could be uniquely determined by the points remaining. Otherwise, print <span class="tex-span"> - 1</span>. </p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4</span>)&nbsp;— the number of vertices that were <span class="tex-font-style-bf">not</span> erased by Wilbur's friend.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 1000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;—the coordinates of the <span class="tex-span"><i>i</i></span>-th vertex that remains. Vertices are given in an arbitrary order.</p><p>It's guaranteed that these points are distinct vertices of some rectangle, that has positive area and which sides are parallel to the coordinate axes.</p>

## Output

<p>Print the area of the initial rectangle if it could be uniquely determined by the points remaining. Otherwise, print <span class="tex-span"> - 1</span>. </p>





```input1
2
0 0
1 1

```




```input2
1
1 1

```




```output1
1

```




```output2
-1

```



## Note

<p>In the first sample, two opposite corners of the initial rectangle are given, and that gives enough information to say that the rectangle is actually a unit square.</p><p>In the second sample there is only one vertex left and this is definitely not enough to uniquely define the area.</p>
