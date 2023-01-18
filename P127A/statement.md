## Description

<div><p>Mr. Scrooge, a very busy man, decided to count the time he wastes on all sorts of useless stuff to evaluate the lost profit. He has already counted the time he wastes sleeping and eating. And now Mr. Scrooge wants to count the time he has wasted signing papers.</p><p>Mr. Scrooge's signature can be represented as a polyline <span class="tex-span"><i>A</i><sub class="lower-index">1</sub><i>A</i><sub class="lower-index">2</sub>... <i>A</i><sub class="lower-index"><i>n</i></sub></span>. Scrooge signs like that: first it places a pen at the point <span class="tex-span"><i>A</i><sub class="lower-index">1</sub></span>, then draws a segment from point <span class="tex-span"><i>A</i><sub class="lower-index">1</sub></span> to point <span class="tex-span"><i>A</i><sub class="lower-index">2</sub></span>, then he draws a segment from point <span class="tex-span"><i>A</i><sub class="lower-index">2</sub></span> to point <span class="tex-span"><i>A</i><sub class="lower-index">3</sub></span> and so on to point <span class="tex-span"><i>A</i><sub class="lower-index"><i>n</i></sub></span>, where he stops signing and takes the pen off the paper. At that the resulting line can intersect with itself and partially repeat itself but Scrooge pays no attention to it and never changes his signing style. As Scrooge makes the signature, he never takes the pen off the paper and his writing speed is constant — <span class="tex-span">50</span> millimeters per second.</p><p>Scrooge signed exactly <span class="tex-span"><i>k</i></span> papers throughout his life and all those signatures look the same.</p><p>Find the total time Scrooge wasted signing the papers.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains the coordinates of the polyline's endpoints. The <span class="tex-span"><i>i</i></span>-th one contains coordinates of the point <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> — integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space.</p><p>All points <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> are different. The absolute value of all coordinates does not exceed <span class="tex-span">20</span>. The coordinates are measured in millimeters.</p></div><div class="output-specification"><p>Print one real number — the total time Scrooges wastes on signing the papers in seconds. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains the coordinates of the polyline's endpoints. The <span class="tex-span"><i>i</i></span>-th one contains coordinates of the point <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> — integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space.</p><p>All points <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> are different. The absolute value of all coordinates does not exceed <span class="tex-span">20</span>. The coordinates are measured in millimeters.</p>

## Output

<p>Print one real number — the total time Scrooges wastes on signing the papers in seconds. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 1
0 0
10 0

```




```input2
5 10
3 1
-5 6
-2 -1
3 2
10 0

```




```input3
6 10
5 0
4 0
6 0
3 0
7 0
2 0

```




```output1
0.200000000
```




```output2
6.032163204
```




```output3
3.000000000
```


