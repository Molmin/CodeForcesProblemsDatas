## Description

<div><p>The Cartesian coordinate system is set in the sky. There you can see <span class="tex-span"><i>n</i></span> stars, the <span class="tex-span"><i>i</i></span>-th has coordinates (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>), a maximum brightness <span class="tex-span"><i>c</i></span>, equal for all stars, and an initial brightness <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i></span>).</p><p>Over time the stars twinkle. At moment <span class="tex-span">0</span> the <span class="tex-span"><i>i</i></span>-th star has brightness <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. Let at moment <span class="tex-span"><i>t</i></span> some star has brightness <span class="tex-span"><i>x</i></span>. Then at moment <span class="tex-span">(<i>t</i> + 1)</span> this star will have brightness <span class="tex-span"><i>x</i> + 1</span>, if <span class="tex-span"><i>x</i> + 1 ≤ <i>c</i></span>, and <span class="tex-span">0</span>, otherwise.</p><p>You want to look at the sky <span class="tex-span"><i>q</i></span> times. In the <span class="tex-span"><i>i</i></span>-th time you will look at the moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and you will see a rectangle with sides parallel to the coordinate axes, the lower left corner has coordinates (<span class="tex-span"><i>x</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1<i>i</i></sub></span>) and the upper right&nbsp;— (<span class="tex-span"><i>x</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2<i>i</i></sub></span>). For each view, you want to know the total brightness of the stars lying in the viewed rectangle.</p><p>A star lies in a rectangle if it lies on its border or lies strictly inside it.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10</span>)&nbsp;— the number of the stars, the number of the views and the maximum brightness of the stars.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the stars description. The <span class="tex-span"><i>i</i></span>-th from these lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i> ≤ 10</span>)&nbsp;— the coordinates of <span class="tex-span"><i>i</i></span>-th star and its initial brightness.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the views description. The <span class="tex-span"><i>i</i></span>-th from these lines contains five integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2<i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1<i>i</i></sub> &lt; <i>x</i><sub class="lower-index">2<i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1<i>i</i></sub> &lt; <i>y</i><sub class="lower-index">2<i>i</i></sub> ≤ 100</span>)&nbsp;— the moment of the <span class="tex-span"><i>i</i></span>-th view and the coordinates of the viewed rectangle.</p></div><div class="output-specification"><p>For each view print the total brightness of the viewed stars.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span>, <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10</span>)&nbsp;— the number of the stars, the number of the views and the maximum brightness of the stars.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the stars description. The <span class="tex-span"><i>i</i></span>-th from these lines contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i> ≤ 10</span>)&nbsp;— the coordinates of <span class="tex-span"><i>i</i></span>-th star and its initial brightness.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the views description. The <span class="tex-span"><i>i</i></span>-th from these lines contains five integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1<i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2<i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1<i>i</i></sub> &lt; <i>x</i><sub class="lower-index">2<i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1<i>i</i></sub> &lt; <i>y</i><sub class="lower-index">2<i>i</i></sub> ≤ 100</span>)&nbsp;— the moment of the <span class="tex-span"><i>i</i></span>-th view and the coordinates of the viewed rectangle.</p>

## Output

<p>For each view print the total brightness of the viewed stars.</p>





```input1
2 3 3
1 1 1
3 2 0
2 1 1 2 2
0 2 1 4 5
5 1 1 5 5

```




```input2
3 4 5
1 1 2
2 3 0
3 3 1
0 1 1 100 100
1 2 2 4 4
2 2 1 4 7
1 50 50 51 51

```




```output1
3
0
3

```




```output2
3
3
5
0

```



## Note

<p>Let's consider the first example.</p><p>At the first view, you can see only the first star. At moment <span class="tex-span">2</span> its brightness is <span class="tex-span">3</span>, so the answer is <span class="tex-span">3</span>.</p><p>At the second view, you can see only the second star. At moment <span class="tex-span">0</span> its brightness is <span class="tex-span">0</span>, so the answer is <span class="tex-span">0</span>.</p><p>At the third view, you can see both stars. At moment <span class="tex-span">5</span> brightness of the first is <span class="tex-span">2</span>, and brightness of the second is <span class="tex-span">1</span>, so the answer is <span class="tex-span">3</span>.</p>
