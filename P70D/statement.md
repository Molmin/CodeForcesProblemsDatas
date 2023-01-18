## Description

<div><p>Once a walrus professor Plato asked his programming students to perform the following practical task. </p><p>The students had to implement such a data structure that would support a convex hull on some set of points <span class="tex-span"><i>S</i></span>. The input to the program had <span class="tex-span"><i>q</i></span> queries of two types: </p><p>1. Add a point with coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span> into the set <span class="tex-span"><i>S</i></span>. Note that in this case the convex hull of <span class="tex-span"><i>S</i></span> could have changed, and could have remained the same. </p><p>2. Say whether a point with coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span> belongs to an area limited by the convex hull, including the border. </p><p>All the students coped with the task. What about you?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">4 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). </p><p>Then follow <span class="tex-span"><i>q</i></span> lines in the following way: "<span class="tex-span"><i>t</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>", where <span class="tex-span"><i>t</i></span> is the query type (1 or 2), and <span class="tex-span">(<i>x</i>, <i>y</i>)</span> are the coordinates of the point (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are integers). </p><p>There is at least one query of type 2.</p><p>It is guaranteed that the three queries of the first type follow first and the points given in the queries form a non-degenerative triangle. Also all the points added in <span class="tex-span"><i>S</i></span> are distinct.</p></div><div class="output-specification"><p>For each query of the second type print one string containing "<span class="tex-font-style-tt">YES</span>", if the point lies inside the convex hull or on its border. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">4 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>). </p><p>Then follow <span class="tex-span"><i>q</i></span> lines in the following way: "<span class="tex-span"><i>t</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>", where <span class="tex-span"><i>t</i></span> is the query type (1 or 2), and <span class="tex-span">(<i>x</i>, <i>y</i>)</span> are the coordinates of the point (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are integers). </p><p>There is at least one query of type 2.</p><p>It is guaranteed that the three queries of the first type follow first and the points given in the queries form a non-degenerative triangle. Also all the points added in <span class="tex-span"><i>S</i></span> are distinct.</p>

## Output

<p>For each query of the second type print one string containing "<span class="tex-font-style-tt">YES</span>", if the point lies inside the convex hull or on its border. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
8
1 0 0
1 2 0
1 2 2
2 1 0
1 0 2
2 1 1
2 2 1
2 20 -1

```




```output1
YES
YES
YES
NO

```


