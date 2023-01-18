## Description

<div><p>There is a right triangle with legs of length <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Your task is to determine whether it is possible to locate the triangle on the plane in such a way that none of its sides is parallel to the coordinate axes. All the vertices must have integer coordinates. If there exists such a location, you have to output the appropriate coordinates of vertices.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 1000</span>), separated by a single space.</p></div><div class="output-specification"><p>In the first line print either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" (without the quotes) depending on whether the required location exists. If it does, print in the next three lines three pairs of integers — the coordinates of the triangle vertices, one pair per line. The coordinates must be integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> in their absolute value.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 1000</span>), separated by a single space.</p>

## Output

<p>In the first line print either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" (without the quotes) depending on whether the required location exists. If it does, print in the next three lines three pairs of integers — the coordinates of the triangle vertices, one pair per line. The coordinates must be integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> in their absolute value.</p>





```input1
1 1

```




```input2
5 5

```




```input3
5 10

```




```output1
NO

```




```output2
YES
2 1
5 5
-2 4

```




```output3
YES
-10 4
-2 -2
1 2

```


