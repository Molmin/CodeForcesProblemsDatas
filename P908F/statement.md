## Description

<div><p>Roy and Biv have a set of <span class="tex-span"><i>n</i></span> points on the infinite number line.</p><p>Each point has one of 3 colors: red, green, or blue.</p><p>Roy and Biv would like to connect all the points with some edges. Edges can be drawn between any of the two of the given points. The cost of an edge is equal to the distance between the two points it connects.</p><p>They want to do this in such a way that they will both see that all the points are connected (either directly or indirectly).</p><p>However, there is a catch: Roy cannot see the color red and Biv cannot see the color blue.</p><p>Therefore, they have to choose the edges in such a way that if all the red points are removed, the remaining blue and green points are connected (and similarly, if all the blue points are removed, the remaining red and green points are connected).</p><p>Help them compute the minimum cost way to choose edges to satisfy the above constraints.</p></div><div class="input-specification"><p>The first line will contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>), the number of points.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain two tokens <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is an integer, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is a uppercase English letter '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' or '<span class="tex-font-style-tt">B</span>'), denoting the position of the <span class="tex-span"><i>i</i></span>-th point and the color of the <span class="tex-span"><i>i</i></span>-th point. '<span class="tex-font-style-tt">R</span>' means red, '<span class="tex-font-style-tt">G</span>' denotes green, and '<span class="tex-font-style-tt">B</span>' means blue. The positions will be in strictly increasing order.</p></div><div class="output-specification"><p>Print a single integer, the minimum cost way to solve the problem.</p></div>

## Input

<p>The first line will contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300 000</span>), the number of points.</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain two tokens <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is an integer, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is a uppercase English letter '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">G</span>' or '<span class="tex-font-style-tt">B</span>'), denoting the position of the <span class="tex-span"><i>i</i></span>-th point and the color of the <span class="tex-span"><i>i</i></span>-th point. '<span class="tex-font-style-tt">R</span>' means red, '<span class="tex-font-style-tt">G</span>' denotes green, and '<span class="tex-font-style-tt">B</span>' means blue. The positions will be in strictly increasing order.</p>

## Output

<p>Print a single integer, the minimum cost way to solve the problem.</p>





```input1
4
1 G
5 R
10 B
15 G

```




```input2
4
1 G
2 R
3 B
10 G

```




```output1
23

```




```output2
12

```



## Note

<p>In the first sample, it is optimal to draw edges between the points (1,2), (1,4), (3,4). These have costs 4, 14, 5, respectively.</p>
