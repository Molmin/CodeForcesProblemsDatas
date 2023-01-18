## Description

<div><p>You are given <span class="tex-span"><i>n</i></span> points with integer coordinates on the plane. Points are given in a way such that there is no triangle, formed by any three of these <span class="tex-span"><i>n</i></span> points, which area exceeds <span class="tex-span"><i>S</i></span>.</p><p>Alyona tried to construct a triangle with integer coordinates, which contains all <span class="tex-span"><i>n</i></span> points and which area doesn't exceed <span class="tex-span">4<i>S</i></span>, but, by obvious reason, had no success in that. Please help Alyona construct such triangle. Please note that vertices of resulting triangle are not necessarily chosen from <span class="tex-span"><i>n</i></span> given points.</p></div><div class="input-specification"><p>In the first line of the input two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>S</i> ≤ 10<sup class="upper-index">18</sup></span>) are given&nbsp;— the number of points given and the upper bound value of any triangle's area, formed by any three of given <span class="tex-span"><i>n</i></span> points.</p><p>The next <span class="tex-span"><i>n</i></span> lines describes given points: <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them consists of two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>&nbsp;— coordinates of <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> point.</p><p>It is guaranteed that there is at least one triple of points not lying on the same line.</p></div><div class="output-specification"><p>Print the coordinates of three points&nbsp;— vertices of a triangle which contains all <span class="tex-span"><i>n</i></span> points and which area doesn't exceed <span class="tex-span">4<i>S</i></span>.</p><p>Coordinates of every triangle's vertex should be printed on a separate line, every coordinate pair should be separated by a single space. Coordinates should be an integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> by absolute value.</p><p>It is guaranteed that there is at least one desired triangle. If there is more than one answer, print any of them.</p></div>

## Input

<p>In the first line of the input two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>S</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>S</i> ≤ 10<sup class="upper-index">18</sup></span>) are given&nbsp;— the number of points given and the upper bound value of any triangle's area, formed by any three of given <span class="tex-span"><i>n</i></span> points.</p><p>The next <span class="tex-span"><i>n</i></span> lines describes given points: <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> of them consists of two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup>)</span>&nbsp;— coordinates of <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> point.</p><p>It is guaranteed that there is at least one triple of points not lying on the same line.</p>

## Output

<p>Print the coordinates of three points&nbsp;— vertices of a triangle which contains all <span class="tex-span"><i>n</i></span> points and which area doesn't exceed <span class="tex-span">4<i>S</i></span>.</p><p>Coordinates of every triangle's vertex should be printed on a separate line, every coordinate pair should be separated by a single space. Coordinates should be an integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> by absolute value.</p><p>It is guaranteed that there is at least one desired triangle. If there is more than one answer, print any of them.</p>





```input1
4 1
0 0
1 0
0 1
1 1

```




```output1
-1 0
2 0
0 2
```



## Note

<center> <img class="tex-graphics" src="file://5bwaUJ6L.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
