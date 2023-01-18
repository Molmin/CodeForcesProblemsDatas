## Description

<div><p>There is a meteor shower on the sky and there are <span class="tex-span"><i>n</i></span> meteors. The sky can be viewed as a 2D Euclid Plane and the meteor is point on this plane. </p><p>Fox Ciel looks at the sky. She finds out that the orbit of each meteor is a straight line, and each meteor has a constant velocity. Now Ciel wants to know: what is the maximum number of <span class="tex-font-style-bf">meteors</span> such that any pair met at the same position at a certain time? Note that the time is not limited and can be also negative. The meteors will never collide when they appear at the same position at the same time.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains six integers: <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> — the description of a meteor's orbit: at time <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, the current meteor is located at the point (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) and at time <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, the meteor is located at point (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>) (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>t</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup>;&nbsp;<i>t</i><sub class="lower-index">1</sub> ≠ <i>t</i><sub class="lower-index">2</sub></span>). </p><p>There will be no two meteors are always in the same position for any time.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of meteors such that any pair met at the same position at a certain time.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). Each of the next <span class="tex-span"><i>n</i></span> lines contains six integers: <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub></span> — the description of a meteor's orbit: at time <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, the current meteor is located at the point (<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>) and at time <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, the meteor is located at point (<span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>) (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>t</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup>;&nbsp;<i>t</i><sub class="lower-index">1</sub> ≠ <i>t</i><sub class="lower-index">2</sub></span>). </p><p>There will be no two meteors are always in the same position for any time.</p>

## Output

<p>Print a single integer — the maximum number of meteors such that any pair met at the same position at a certain time.</p>





```input1
2
0 0 1 1 0 2
0 1 0 1 2 0

```




```input2
3
-1 -1 0 3 3 0
0 2 -1 -1 3 -2
-2 0 -1 6 0 3

```




```input3
4
0 0 0 1 0 1
0 0 1 1 1 1
0 1 1 1 1 0
0 1 0 1 0 0

```




```input4
1
0 0 0 1 0 0

```




```output1
2

```




```output2
3

```




```output3
1

```




```output4
1

```



## Note

<p>In example 1, meteor 1 and 2 meet in <span class="tex-span"><i>t</i></span>=-1 at (0, 0).</p><center><img class="tex-graphics" src="file://gOi3R8Y6.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In example 2, meteor 1 and 2 meet in <span class="tex-span"><i>t</i></span>=1 at (1, 0), meteor 1 and 3 meet in <span class="tex-span"><i>t</i></span>=0 at (0, 0) and meteor 2 and 3 meet in <span class="tex-span"><i>t</i></span>=2 at (0, 1).</p><center><img class="tex-graphics" src="file://6xuTfK5B.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In example 3, no two meteor meet.</p><center><img class="tex-graphics" src="file://sDInRULB.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In example 4, there is only 1 meteor, and its velocity is zero.</p><center><img class="tex-graphics" src="file://wYu32Ssm.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>If your browser doesn't support animation png, please see the gif version here: </p><p>http://assets.codeforces.com/images/388e/example1.gif</p><p>http://assets.codeforces.com/images/388e/example2.gif</p><p>http://assets.codeforces.com/images/388e/example3.gif</p><p>http://assets.codeforces.com/images/388e/example4.gif</p>
