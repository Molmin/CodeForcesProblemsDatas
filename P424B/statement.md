## Description

<div><p>The administration of the Tomsk Region firmly believes that it's time to become a megacity (that is, get population of one million). Instead of improving the demographic situation, they decided to achieve its goal by expanding the boundaries of the city.</p><p>The city of Tomsk can be represented as point on the plane with coordinates (<span class="tex-span">0</span>; <span class="tex-span">0</span>). The city is surrounded with <span class="tex-span"><i>n</i></span> other locations, the <span class="tex-span"><i>i</i></span>-th one has coordinates (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>) with the population of <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> people. You can widen the city boundaries to a circle of radius <span class="tex-span"><i>r</i></span>. In such case all locations inside the circle and on its border are included into the city.</p><p>Your goal is to write a program that will determine the minimum radius <span class="tex-span"><i>r</i></span>, to which is necessary to expand the boundaries of Tomsk, so that it becomes a megacity.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>; <span class="tex-span">1 ≤ <i>s</i> &lt; 10<sup class="upper-index">6</sup></span>) — the number of locatons around Tomsk city and the population of the city. Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line contains three integers — the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> coordinate values of the <span class="tex-span"><i>i</i></span>-th location and the number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> of people in it (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">6</sup></span>). Each coordinate is an integer and doesn't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in its absolute value.</p><p>It is guaranteed that no two locations are at the same point and no location is at point (<span class="tex-span">0;&nbsp;0</span>).</p></div><div class="output-specification"><p>In the output, print "<span class="tex-font-style-tt">-1</span>" (without the quotes), if Tomsk won't be able to become a megacity. Otherwise, in the first line print a single real number — the minimum radius of the circle that the city needs to expand to in order to become a megacity.</p><p>The answer is considered correct if the absolute or relative error don't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>; <span class="tex-span">1 ≤ <i>s</i> &lt; 10<sup class="upper-index">6</sup></span>) — the number of locatons around Tomsk city and the population of the city. Then <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line contains three integers — the <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> coordinate values of the <span class="tex-span"><i>i</i></span>-th location and the number <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> of people in it (<span class="tex-span">1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">6</sup></span>). Each coordinate is an integer and doesn't exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> in its absolute value.</p><p>It is guaranteed that no two locations are at the same point and no location is at point (<span class="tex-span">0;&nbsp;0</span>).</p>

## Output

<p>In the output, print "<span class="tex-font-style-tt">-1</span>" (without the quotes), if Tomsk won't be able to become a megacity. Otherwise, in the first line print a single real number — the minimum radius of the circle that the city needs to expand to in order to become a megacity.</p><p>The answer is considered correct if the absolute or relative error don't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4 999998
1 1 1
2 2 1
3 3 1
2 -2 1

```




```input2
4 999998
1 1 2
2 2 1
3 3 1
2 -2 1

```




```input3
2 1
1 1 999997
2 2 1

```




```output1
2.8284271

```




```output2
1.4142136

```




```output3
-1
```


