## Description

<div><p>You are given a set of points on a plane with positive integer coordinates. Find a triangle of minimum area with vertices in points <span class="tex-span">(0, 0)</span>, <span class="tex-span">(<i>A</i>, 0)</span> and <span class="tex-span">(0, <i>B</i>)</span> (<span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are unknown positive integers) that contains all the given points inside it (points on the edges count towards being inside).</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>) — the number of points. The following <span class="tex-span"><i>N</i></span> lines contain pairs of numbers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> (<span class="tex-span">1 ≤ <i>X</i>, <i>Y</i> ≤ 100</span>) - the coordinates of the points. All points are distinct.</p></div><div class="output-specification"><p>Output one floating-point number — the minimal area of the triangle. The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>) — the number of points. The following <span class="tex-span"><i>N</i></span> lines contain pairs of numbers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> (<span class="tex-span">1 ≤ <i>X</i>, <i>Y</i> ≤ 100</span>) - the coordinates of the points. All points are distinct.</p>

## Output

<p>Output one floating-point number — the minimal area of the triangle. The answer is considered to be correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
2
1 1
1 3

```




```input2
2
2 1
1 2

```




```output1
6.0

```




```output2
4.5

```


