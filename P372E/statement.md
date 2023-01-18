## Description

<div><p>There are a set of points <span class="tex-span"><i>S</i></span> on the plane. This set doesn't contain the origin <span class="tex-span"><i>O</i>(0, 0)</span>, and for each two distinct points in the set <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>, the triangle <span class="tex-span"><i>OAB</i></span> has strictly positive area.</p><p>Consider a set of pairs of points <span class="tex-span">(<i>P</i><sub class="lower-index">1</sub>, <i>P</i><sub class="lower-index">2</sub>), (<i>P</i><sub class="lower-index">3</sub>, <i>P</i><sub class="lower-index">4</sub>), ..., (<i>P</i><sub class="lower-index">2<i>k</i> - 1</sub>, <i>P</i><sub class="lower-index">2<i>k</i></sub>)</span>. We'll call the set <span class="tex-font-style-it">good</span> if and only if:</p><ul> <li> <span class="tex-span"><i>k</i> ≥ 2</span>. </li><li> All <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span> are distinct, and each <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span> is an element of <span class="tex-span"><i>S</i></span>. </li><li> For any two pairs <span class="tex-span">(<i>P</i><sub class="lower-index">2<i>i</i> - 1</sub>, <i>P</i><sub class="lower-index">2<i>i</i></sub>)</span> and <span class="tex-span">(<i>P</i><sub class="lower-index">2<i>j</i> - 1</sub>, <i>P</i><sub class="lower-index">2<i>j</i></sub>)</span>, the circumcircles of triangles <span class="tex-span"><i>OP</i><sub class="lower-index">2<i>i</i> - 1</sub><i>P</i><sub class="lower-index">2<i>j</i> - 1</sub></span> and <span class="tex-span"><i>OP</i><sub class="lower-index">2<i>i</i></sub><i>P</i><sub class="lower-index">2<i>j</i></sub></span> have a single common point, and the circumcircle of triangles <span class="tex-span"><i>OP</i><sub class="lower-index">2<i>i</i> - 1</sub><i>P</i><sub class="lower-index">2<i>j</i></sub></span> and <span class="tex-span"><i>OP</i><sub class="lower-index">2<i>i</i></sub><i>P</i><sub class="lower-index">2<i>j</i> - 1</sub></span> have a single common point. </li></ul><p>Calculate the number of good sets of pairs modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the number of points in <span class="tex-span"><i>S</i></span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>| ≤ 50;&nbsp;1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 50;&nbsp;(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>) ≠ (0, 0))</span>. These integers represent a point <img align="middle" class="tex-formula" src="file://DSDtVLGD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>No two points coincide.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span> — the number of points in <span class="tex-span"><i>S</i></span>. Each of the next <span class="tex-span"><i>n</i></span> lines contains four integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>|, |<i>c</i><sub class="lower-index"><i>i</i></sub>| ≤ 50;&nbsp;1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 50;&nbsp;(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>) ≠ (0, 0))</span>. These integers represent a point <img align="middle" class="tex-formula" src="file://DSDtVLGD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>No two points coincide.</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
10
-46 46 0 36
0 20 -24 48
-50 50 -49 49
-20 50 8 40
-15 30 14 28
4 10 -4 5
6 15 8 10
-20 50 -3 15
4 34 -16 34
16 34 2 17

```




```input2
10
30 30 -26 26
0 15 -36 36
-28 28 -34 34
10 10 0 4
-8 20 40 50
9 45 12 30
6 15 7 35
36 45 -8 20
-16 34 -4 34
4 34 8 17

```




```input3
10
0 20 38 38
-30 30 -13 13
-11 11 16 16
30 30 0 37
6 30 -4 10
6 15 12 15
-4 5 -10 25
-16 20 4 10
8 17 -2 17
16 34 2 17

```




```output1
2

```




```output2
4

```




```output3
10

```


