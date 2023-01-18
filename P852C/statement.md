## Description

<div><p>Bill is a famous mathematician in BubbleLand. Thanks to his revolutionary math discoveries he was able to make enough money to build a beautiful house. Unfortunately, for not paying property tax on time, court decided to punish Bill by making him lose a part of his property.</p><p>Bill’s property can be observed as a convex regular <span class="tex-span">2<i>n</i></span>-sided polygon <span class="tex-span"><i>A</i><sub class="lower-index">0</sub> <i>A</i><sub class="lower-index">1</sub>... <i>A</i><sub class="lower-index">2<i>n</i> - 1</sub> <i>A</i><sub class="lower-index">2<i>n</i></sub>,  <i>A</i><sub class="lower-index">2<i>n</i></sub> =  <i>A</i><sub class="lower-index">0</sub></span>, with sides of the exactly 1 meter in length. </p><p>Court rules for removing part of his property are as follows:</p><ul>  <li> Split every edge <span class="tex-span"><i>A</i><sub class="lower-index"><i>k</i></sub> <i>A</i><sub class="lower-index"><i>k</i> + 1</sub>,  <i>k</i> = 0... 2<i>n</i> - 1</span> in <span class="tex-span"><i>n</i></span> equal parts of size <span class="tex-span">1 / <i>n</i></span> with points <span class="tex-span"><i>P</i><sub class="lower-index">0</sub>, <i>P</i><sub class="lower-index">1</sub>, ..., <i>P</i><sub class="lower-index"><i>n</i> - 1</sub></span>  </li><li> On every edge <span class="tex-span"><i>A</i><sub class="lower-index">2<i>k</i></sub> <i>A</i><sub class="lower-index">2<i>k</i> + 1</sub>,  <i>k</i> = 0... <i>n</i> - 1</span> court will choose one point <span class="tex-span"><i>B</i><sub class="lower-index">2<i>k</i></sub> =  <i>P</i><sub class="lower-index"><i>i</i></sub></span> for some <span class="tex-span"><i>i</i> = 0, ...,  <i>n</i> - 1</span> such that <img align="middle" class="tex-formula" src="file://GdC9ATTd.png" style="max-width: 100.0%;max-height: 100.0%;">  </li><li> On every edge <span class="tex-span"><i>A</i><sub class="lower-index">2<i>k</i> + 1</sub><i>A</i><sub class="lower-index">2<i>k</i> + 2</sub>,  <i>k</i> = 0...<i>n</i> - 1</span> Bill will choose one point <span class="tex-span"><i>B</i><sub class="lower-index">2<i>k</i> + 1</sub> =  <i>P</i><sub class="lower-index"><i>i</i></sub></span> for some <span class="tex-span"><i>i</i> = 0, ...,  <i>n</i> - 1</span> such that <img align="middle" class="tex-formula" src="file://GkzWNDvY.png" style="max-width: 100.0%;max-height: 100.0%;">  </li><li> Bill gets to keep property inside of <span class="tex-span">2<i>n</i></span>-sided polygon <span class="tex-span"><i>B</i><sub class="lower-index">0</sub> <i>B</i><sub class="lower-index">1</sub>... <i>B</i><sub class="lower-index">2<i>n</i> - 1</sub></span> </li></ul><p>Luckily, Bill found out which <span class="tex-span"><i>B</i><sub class="lower-index">2<i>k</i></sub></span> points the court chose. Even though he is a great mathematician, his house is very big and he has a hard time calculating. Therefore, he is asking you to help him choose points so he maximizes area of property he can keep.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i> (2 ≤ <i>n</i> ≤ 50000)</span>, representing number of edges of <span class="tex-span">2<i>n</i></span>-sided polygon.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integer numbers <span class="tex-span"><i>B</i><sub class="lower-index">2<i>k</i></sub> (0 ≤ <i>B</i><sub class="lower-index">2<i>k</i></sub> ≤ <i>n</i> - 1,  <i>k</i> = 0... <i>n</i> - 1)</span> separated by a single space, representing points the court chose. If <span class="tex-span"><i>B</i><sub class="lower-index">2<i>k</i></sub> = <i>i</i></span>, the court chose point <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span> on side <span class="tex-span"><i>A</i><sub class="lower-index">2<i>k</i></sub> <i>A</i><sub class="lower-index">2<i>k</i> + 1</sub></span>.</p></div><div class="output-specification"><p>Output contains <span class="tex-span"><i>n</i></span> distinct integers separated by a single space representing points <span class="tex-span"><i>B</i><sub class="lower-index">1</sub>, <i>B</i><sub class="lower-index">3</sub>, ..., <i>B</i><sub class="lower-index">2<i>n</i> - 1</sub></span> Bill should choose in order to maximize the property area. If there are multiple solutions that maximize the area, return any of them.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i> (2 ≤ <i>n</i> ≤ 50000)</span>, representing number of edges of <span class="tex-span">2<i>n</i></span>-sided polygon.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integer numbers <span class="tex-span"><i>B</i><sub class="lower-index">2<i>k</i></sub> (0 ≤ <i>B</i><sub class="lower-index">2<i>k</i></sub> ≤ <i>n</i> - 1,  <i>k</i> = 0... <i>n</i> - 1)</span> separated by a single space, representing points the court chose. If <span class="tex-span"><i>B</i><sub class="lower-index">2<i>k</i></sub> = <i>i</i></span>, the court chose point <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span> on side <span class="tex-span"><i>A</i><sub class="lower-index">2<i>k</i></sub> <i>A</i><sub class="lower-index">2<i>k</i> + 1</sub></span>.</p>

## Output

<p>Output contains <span class="tex-span"><i>n</i></span> distinct integers separated by a single space representing points <span class="tex-span"><i>B</i><sub class="lower-index">1</sub>, <i>B</i><sub class="lower-index">3</sub>, ..., <i>B</i><sub class="lower-index">2<i>n</i> - 1</sub></span> Bill should choose in order to maximize the property area. If there are multiple solutions that maximize the area, return any of them.</p>





```input1
3
0 1 2

```




```output1
0 2 1

```



## Note

<p>To maximize area Bill should choose points: <span class="tex-span"><i>B</i><sub class="lower-index">1</sub> = <i>P</i><sub class="lower-index">0</sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index">3</sub> = <i>P</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index">5</sub> = <i>P</i><sub class="lower-index">1</sub></span></p><p><img class="tex-graphics" src="file://E3Wy6hPT.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
