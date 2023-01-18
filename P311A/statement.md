## Description

<div><p>Currently Tiny is learning Computational Geometry. When trying to solve a problem called "The Closest Pair Of Points In The Plane", he found that a code which gave a wrong time complexity got Accepted instead of Time Limit Exceeded.</p><p>The problem is the follows. Given <span class="tex-span"><i>n</i></span> points in the plane, find a pair of points between which the distance is minimized. Distance between <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span> is <img align="middle" class="tex-formula" src="file://vKZqQsXN.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The pseudo code of the unexpected code is as follows:</p><pre class="verbatim"><br>input n<br>for i from 1 to n<br>    input the i-th point's coordinates into p[i]<br>sort array p[] by increasing of x coordinate first and increasing of y coordinate second<br>d=INF        //here INF is a number big enough<br>tot=0<br>for i from 1 to n<br>    for j from (i+1) to n<br>        ++tot<br>        if (p[j].x-p[i].x&gt;=d) then break    //notice that "break" is only to be<br>                                            //out of the loop "for j"<br>        d=min(d,distance(p[i],p[j]))<br>output d<br></pre><p>Here, <span class="tex-span"><i>tot</i></span> can be regarded as the running time of the code. Due to the fact that a computer can only run a limited number of operations per second, <span class="tex-span"><i>tot</i></span> should not be more than <span class="tex-span"><i>k</i></span> in order not to get Time Limit Exceeded.</p><p>You are a great hacker. Would you please help Tiny generate a test data and let the code get Time Limit Exceeded?</p></div><div class="input-specification"><p>A single line which contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>If there doesn't exist such a data which let the given code get TLE, print "<span class="tex-font-style-tt">no solution</span>" (without quotes); else print <span class="tex-span"><i>n</i></span> lines, and the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> representing the coordinates of the <span class="tex-span"><i>i</i></span>-th point.</p><p>The conditions below must be held:</p><ul> <li> All the points must be distinct. </li><li> <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>. </li><li> After running the given code, the value of <span class="tex-span"><i>tot</i></span> should be larger than <span class="tex-span"><i>k</i></span>. </li></ul></div>

## Input

<p>A single line which contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>If there doesn't exist such a data which let the given code get TLE, print "<span class="tex-font-style-tt">no solution</span>" (without quotes); else print <span class="tex-span"><i>n</i></span> lines, and the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>)</span> representing the coordinates of the <span class="tex-span"><i>i</i></span>-th point.</p><p>The conditions below must be held:</p><ul> <li> All the points must be distinct. </li><li> <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>. </li><li> After running the given code, the value of <span class="tex-span"><i>tot</i></span> should be larger than <span class="tex-span"><i>k</i></span>. </li></ul>





```input1
4 3

```




```input2
2 100

```




```output1
0 0
0 1
1 0
1 1

```




```output2
no solution

```


