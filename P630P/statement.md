## Description

<div><p>It was decided in IT City to distinguish successes of local IT companies by awards in the form of stars covered with gold from one side. To order the stars it is necessary to estimate order cost that depends on the area of gold-plating. Write a program that can calculate the area of a star.</p><p>A "star" figure having <span class="tex-span"><i>n</i> ≥ 5</span> corners where <span class="tex-span"><i>n</i></span> is a prime number is constructed the following way. On the circle of radius <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>n</i></span> points are selected so that the distances between the adjacent ones are equal. Then every point is connected by a segment with two maximally distant points. All areas bounded by the segments parts are the figure parts.</p><center> <img class="tex-graphics" src="file://stH4Fx3Y.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> &lt; 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>n</i></span> is prime) and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of the star corners and the radius of the circumcircle correspondingly.</p></div><div class="output-specification"><p>Output one number — the star area. The relative error of your answer should not be greater than <span class="tex-span">10<sup class="upper-index"> - 7</sup></span>.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> &lt; 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>n</i></span> is prime) and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of the star corners and the radius of the circumcircle correspondingly.</p>

## Output

<p>Output one number — the star area. The relative error of your answer should not be greater than <span class="tex-span">10<sup class="upper-index"> - 7</sup></span>.</p>





```input1
7 10

```




```output1
108.395919545675
```


