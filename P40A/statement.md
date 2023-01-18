## Description

<div><p>Not so long ago as a result of combat operations the main Berland place of interest — the magic clock — was damaged. The cannon's balls made several holes in the clock, that's why the residents are concerned about the repair. The magic clock can be represented as an <span class="tex-font-style-bf">infinite</span> Cartesian plane, where the origin corresponds to the clock center. The clock was painted two colors as is shown in the picture:</p><center> <img class="tex-graphics" src="file://aBqKa9p8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The picture shows only the central part of the clock. This coloring naturally extends to infinity.</p><p>The balls can be taken to be points on the plane. Your task is to find the color of the area, damaged by the given ball.</p><p>All the points located on the border of one of the areas have to be considered painted black.</p></div><div class="input-specification"><p>The first and single line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the coordinates of the hole made in the clock by the ball. Each of the numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> has an absolute value that does not exceed <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>Find the required color.</p><p>All the points between which and the origin of coordinates the distance is integral-value are painted black.</p></div>

## Input

<p>The first and single line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the coordinates of the hole made in the clock by the ball. Each of the numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> has an absolute value that does not exceed <span class="tex-span">1000</span>.</p>

## Output

<p>Find the required color.</p><p>All the points between which and the origin of coordinates the distance is integral-value are painted black.</p>





```input1
-2 1

```




```input2
2 1

```




```input3
4 3

```




```output1
white

```




```output2
black

```




```output3
black

```


