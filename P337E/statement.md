## Description

<div><p>A <span class="tex-font-style-it">divisor tree</span> is a rooted tree that meets the following conditions: </p><ul> <li> Each vertex of the tree contains a positive integer number. </li><li> The numbers written in the leaves of the tree are prime numbers. </li><li> For any inner vertex, the number within it is equal to the product of the numbers written in its children. </li></ul><p>Manao has <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. He tries to build a divisor tree which contains each of these numbers. That is, for each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, there should be at least one vertex in the tree which contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Manao loves compact style, but his trees are too large. Help Manao determine the minimum possible number of vertices in the divisor tree sought.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 8</span>). The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p></div><div class="output-specification"><p>Print a single integer — the minimum number of vertices in the divisor tree that contains each of the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 8</span>). The second line contains <span class="tex-span"><i>n</i></span> distinct space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p>

## Output

<p>Print a single integer — the minimum number of vertices in the divisor tree that contains each of the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
2
6 10

```




```input2
4
6 72 8 4

```




```input3
1
7

```




```output1
7

```




```output2
12

```




```output3
1

```



## Note

<p>Sample 1. The smallest divisor tree looks this way: <img class="tex-graphics" src="file://qDtW5qbh.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Sample 2. In this case you can build the following divisor tree: <img class="tex-graphics" src="file://UbrL9OGc.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Sample 3. Note that the tree can consist of a single vertex.</p>
