## Description

<div><p>Recently Luba bought a monitor. Monitor is a rectangular matrix of size <span class="tex-span"><i>n</i> × <i>m</i></span>. But then she started to notice that some pixels cease to work properly. Luba thinks that the monitor will become broken the first moment when it contains a square <span class="tex-span"><i>k</i> × <i>k</i></span> consisting entirely of broken pixels. She knows that <span class="tex-span"><i>q</i></span> pixels are already broken, and for each of them she knows the moment when it stopped working. Help Luba to determine when the monitor became broken (or tell that it's still not broken even after all <span class="tex-span"><i>q</i></span> pixels stopped working).</p></div><div class="input-specification"><p>The first line contains four integer numbers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>q</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 500, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, <i>m</i>), 0 ≤ <i>q</i> ≤ <i>n</i>·<i>m</i>)</span> — the length and width of the monitor, the size of a rectangle such that the monitor is broken if there is a broken rectangle with this size, and the number of broken pixels.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contain three integer numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>, 0 ≤ <i>t</i><sub class="lower-index"></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — coordinates of <span class="tex-span"><i>i</i></span>-th broken pixel (its row and column in matrix) and the moment it stopped working. Each pixel is listed at most once.</p><p>We consider that pixel is already broken at moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print one number — the minimum moment the monitor became broken, or "-1" if it's still not broken after these <span class="tex-span"><i>q</i></span> pixels stopped working.</p></div>

## Input

<p>The first line contains four integer numbers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i>, <i>q</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 500, 1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, <i>m</i>), 0 ≤ <i>q</i> ≤ <i>n</i>·<i>m</i>)</span> — the length and width of the monitor, the size of a rectangle such that the monitor is broken if there is a broken rectangle with this size, and the number of broken pixels.</p><p>Each of next <span class="tex-span"><i>q</i></span> lines contain three integer numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>, 0 ≤ <i>t</i><sub class="lower-index"></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — coordinates of <span class="tex-span"><i>i</i></span>-th broken pixel (its row and column in matrix) and the moment it stopped working. Each pixel is listed at most once.</p><p>We consider that pixel is already broken at moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print one number — the minimum moment the monitor became broken, or "-1" if it's still not broken after these <span class="tex-span"><i>q</i></span> pixels stopped working.</p>





```input1
2 3 2 5
2 1 8
2 2 8
1 2 1
1 3 4
2 3 2

```




```input2
3 3 2 5
1 2 2
2 2 1
2 3 5
3 2 10
2 1 100

```




```output1
8

```




```output2
-1

```


