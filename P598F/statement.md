## Description

<div><p>Given simple (without self-intersections) <span class="tex-span"><i>n</i></span>-gon. It is not necessary convex. Also you are given <span class="tex-span"><i>m</i></span> lines. For each line find the length of common part of the line and the <span class="tex-span"><i>n</i></span>-gon.</p><p>The boundary of <span class="tex-span"><i>n</i></span>-gon belongs to polygon. It is possible that <span class="tex-span"><i>n</i></span>-gon contains 180-degree angles.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000;1 ≤ <i>m</i> ≤ 100</span>). The following <span class="tex-span"><i>n</i></span> lines contain coordinates of polygon vertices (in clockwise or counterclockwise direction). All vertices are distinct.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain line descriptions. Each of them contains two distict points of a line by their coordinates.</p><p>All given in the input coordinates are real numbers, given with at most two digits after decimal point. They do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> by absolute values.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the length of common part of the given <span class="tex-span"><i>n</i></span>-gon and the <span class="tex-span"><i>i</i></span>-th line. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 1000;1 ≤ <i>m</i> ≤ 100</span>). The following <span class="tex-span"><i>n</i></span> lines contain coordinates of polygon vertices (in clockwise or counterclockwise direction). All vertices are distinct.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain line descriptions. Each of them contains two distict points of a line by their coordinates.</p><p>All given in the input coordinates are real numbers, given with at most two digits after decimal point. They do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> by absolute values.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain the length of common part of the given <span class="tex-span"><i>n</i></span>-gon and the <span class="tex-span"><i>i</i></span>-th line. The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4 3
0 0
1 0
1 1
0 1
0 0 1 1
0 0 0 1
0 0 1 -1

```




```output1
1.41421356237309514547
1.00000000000000000000
0.00000000000000000000

```


