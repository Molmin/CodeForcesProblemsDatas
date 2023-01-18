## Description

<div><p>Imagine you have an infinite 2D plane with Cartesian coordinate system. Some of the integral points are blocked, and others are not. Two integral points <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> on the plane are 4-connected if and only if:</p><ul> <li> the Euclidean distance between <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> is one unit and neither <span class="tex-span"><i>A</i></span> nor <span class="tex-span"><i>B</i></span> is blocked; </li><li> or there is some integral point <span class="tex-span"><i>C</i></span>, such that <span class="tex-span"><i>A</i></span> is 4-connected with <span class="tex-span"><i>C</i></span>, and <span class="tex-span"><i>C</i></span> is 4-connected with <span class="tex-span"><i>B</i></span>. </li></ul><p>Let's assume that the plane doesn't contain blocked points. Consider all the integral points of the plane whose Euclidean distance from the origin is no more than <span class="tex-span"><i>n</i></span>, we'll name these points special. Chubby Yang wants to get the following property: no special point is 4-connected to some non-special point. To get the property she can pick some integral points of the plane and make them blocked. What is the minimum number of points she needs to pick?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 4·10<sup class="upper-index">7</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of points that should be blocked.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(0 ≤ <i>n</i> ≤ 4·10<sup class="upper-index">7</sup>)</span>.</p>

## Output

<p>Print a single integer — the minimum number of points that should be blocked.</p>





```input1
1

```




```input2
2

```




```input3
3

```




```output1
4

```




```output2
8

```




```output3
16

```


