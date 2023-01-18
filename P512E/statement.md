## Description

<div><p>Fox Ciel just designed a puzzle game called "Polygon"! It is played using triangulations of a regular <span class="tex-span"><i>n</i></span>-edge polygon. The goal is to transform one <span class="tex-font-style-underline">triangulation</span> to another by some tricky rules.</p><center><img class="tex-graphics" src="file://R5CT0dsa.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p><span class="tex-font-style-underline">Triangulation</span> of an <span class="tex-span"><i>n</i></span>-edge poylgon is a set of <span class="tex-span"><i>n</i> - 3</span> diagonals satisfying the condition that no two diagonals share a common internal point.</p><p>For example, the initial state of the game may look like (a) in above figure. And your goal may look like (c). In each step you can choose a diagonal inside the polygon (but not the one of edges of the polygon) and <span class="tex-font-style-underline">flip</span> this diagonal. </p><p>Suppose you are going to <span class="tex-font-style-underline">flip</span> a diagonal <span class="tex-span"><i>a</i> – <i>b</i></span>. There always exist two triangles sharing <span class="tex-span"><i>a</i> – <i>b</i></span> as a side, let's denote them as <span class="tex-span"><i>a</i> – <i>b</i> – <i>c</i></span> and <span class="tex-span"><i>a</i> – <i>b</i> – <i>d</i></span>. As a result of this operation, the diagonal <span class="tex-span"><i>a</i> – <i>b</i></span> is replaced by a diagonal <span class="tex-span"><i>c</i> – <i>d</i></span>. It can be easily proven that after <span class="tex-font-style-underline">flip</span> operation resulting set of diagonals is still a <span class="tex-font-style-underline">triangulation</span> of the polygon.</p><p>So in order to solve above case, you may first <span class="tex-font-style-underline">flip</span> diagonal <span class="tex-span">6 – 3</span>, it will be replaced by diagonal <span class="tex-span">2 – 4</span>. Then you <span class="tex-font-style-underline">flip</span> diagonal <span class="tex-span">6 – 4</span> and get figure (c) as result.</p><p>Ciel just proved that for any starting and destination triangulations this game has a solution. She wants you to solve it in no more than <span class="tex-span">20 000</span> steps for any puzzle satisfying <span class="tex-span"><i>n</i> ≤ 1000</span>.</p></div><div class="input-specification"><p>The first line contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>), number of edges of the regular polygon. </p><p>Then follows two groups of <span class="tex-span">(<i>n</i> - 3)</span> lines describing the original triangulation and goal triangulation.</p><p>Description of each triangulation consists of <span class="tex-span">(<i>n</i> - 3)</span> lines. Each line contains 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing a diagonal <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> – <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that both original and goal triangulations are correct (i. e. no two diagonals share a common internal point in both of these triangulations).</p></div><div class="output-specification"><p>First, output an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 20, 000</span>): number of steps.</p><p>Then output <span class="tex-span"><i>k</i></span> lines, each containing 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>: the endpoints of a diagonal you are going to flip at step <span class="tex-span"><i>i</i></span>. You may output <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in any order.</p><p>If there are several possible solutions, output any of them.</p></div>

## Input

<p>The first line contain an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>), number of edges of the regular polygon. </p><p>Then follows two groups of <span class="tex-span">(<i>n</i> - 3)</span> lines describing the original triangulation and goal triangulation.</p><p>Description of each triangulation consists of <span class="tex-span">(<i>n</i> - 3)</span> lines. Each line contains 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing a diagonal <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> – <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that both original and goal triangulations are correct (i. e. no two diagonals share a common internal point in both of these triangulations).</p>

## Output

<p>First, output an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 20, 000</span>): number of steps.</p><p>Then output <span class="tex-span"><i>k</i></span> lines, each containing 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>: the endpoints of a diagonal you are going to flip at step <span class="tex-span"><i>i</i></span>. You may output <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in any order.</p><p>If there are several possible solutions, output any of them.</p>





```input1
4
1 3
2 4

```




```input2
6
2 6
3 6
4 6
6 2
5 2
4 2

```




```input3
8
7 1
2 7
7 3
6 3
4 6
6 1
6 2
6 3
6 4
6 8

```




```output1
1
1 3

```




```output2
2
6 3
6 4

```




```output3
3
7 3
7 2
7 1
```



## Note

<p>Sample test 2 is discussed above and shown on the picture.</p>
