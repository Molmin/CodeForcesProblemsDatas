## Description

<div><p>You are given a tree <span class="tex-span"><i>T</i></span> consisting of <span class="tex-span"><i>n</i></span> vertices. A number is written on each vertex; the number written on vertex <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Let's denote the function <span class="tex-span"><i>I</i>(<i>x</i>, <i>y</i>)</span> as the difference between maximum and minimum value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> on a simple path connecting vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p><p>Your task is to calculate <img align="middle" class="tex-formula" src="file://Nel30ekQ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the numbers written on the vertices.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. Each line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> denoting an edge connecting vertex <span class="tex-span"><i>x</i></span> and vertex <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i> ≠ <i>y</i></span>). It is guaranteed that these edges denote a tree.</p></div><div class="output-specification"><p>Print one number equal to <img align="middle" class="tex-formula" src="file://w6Uizxt3.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of vertices in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the numbers written on the vertices.</p><p>Then <span class="tex-span"><i>n</i> - 1</span> lines follow. Each line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> denoting an edge connecting vertex <span class="tex-span"><i>x</i></span> and vertex <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i> ≠ <i>y</i></span>). It is guaranteed that these edges denote a tree.</p>

## Output

<p>Print one number equal to <img align="middle" class="tex-formula" src="file://w6Uizxt3.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4
2 2 3 1
1 2
1 3
1 4

```




```output1
6

```


