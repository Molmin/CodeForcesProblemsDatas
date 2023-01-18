## Description

<div><p><span class="tex-font-style-it">Firecrackers scare Nian the monster, but they're wayyyyy too noisy! Maybe fireworks make a nice complement.</span></p><p>Little Tommy is watching a firework show. As circular shapes spread across the sky, a splendid view unfolds on the night of Lunar New Year's eve.</p><p>A wonder strikes Tommy. How many regions are formed by the circles on the sky? We consider the sky as a flat plane. A region is a connected part of the plane with positive area, whose bound consists of parts of bounds of the circles and is a curve or several curves without self-intersections, and that does not contain any curve other than its boundaries. Note that exactly one of the regions extends infinitely.</p></div><div class="input-specification"><p>The first line of input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3</span>), denoting the number of circles.</p><p>The following <span class="tex-span"><i>n</i></span> lines each contains three space-separated integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span"> - 10 ≤ <i>x</i>, <i>y</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10</span>), describing a circle whose center is <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and the radius is <span class="tex-span"><i>r</i></span>. No two circles have the same <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>r</i></span> at the same time.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of regions on the plane.</p></div>

## Input

<p>The first line of input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3</span>), denoting the number of circles.</p><p>The following <span class="tex-span"><i>n</i></span> lines each contains three space-separated integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span"> - 10 ≤ <i>x</i>, <i>y</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10</span>), describing a circle whose center is <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and the radius is <span class="tex-span"><i>r</i></span>. No two circles have the same <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>r</i></span> at the same time.</p>

## Output

<p>Print a single integer&nbsp;— the number of regions on the plane.</p>





```input1
3
0 0 1
2 0 1
4 0 1

```




```input2
3
0 0 2
3 0 2
6 0 2

```




```input3
3
0 0 2
2 0 2
1 1 2

```




```output1
4

```




```output2
6

```




```output3
8

```



## Note

<p>For the first example,</p><center> <img class="tex-graphics" src="file://Nmcs93f2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the second example,</p><center> <img class="tex-graphics" src="file://ya3fqaLD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the third example,</p><center> <img class="tex-graphics" src="file://YMkcDmHZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
