## Description

<div><p>Jzzhu has two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. He calls an integer point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of a plane special if <span class="tex-span">0 ≤ <i>x</i> ≤ <i>n</i></span> and <span class="tex-span">0 ≤ <i>y</i> ≤ <i>m</i></span>. Jzzhu defines a unit square as a square with corners at points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> + 1, <i>y</i> + 1)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>, where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are some integers.</p><p>Let's look at all the squares (their sides not necessarily parallel to the coordinate axes) with corners at the special points. For each such square Jzzhu paints a dot in every unit square that is fully inside it. After that some unit squares can contain several dots. Now Jzzhu wonders, how many dots he has painted on the plane. Find this number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of tests.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains the description of the test: two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the value of variables for the current test.</p></div><div class="output-specification"><p>For each test output the total number of dots modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of tests.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains the description of the test: two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the value of variables for the current test.</p>

## Output

<p>For each test output the total number of dots modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
4
1 3
2 2
2 5
3 4

```




```output1
3
8
26
58

```


