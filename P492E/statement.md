## Description

<div><p>Vanya decided to walk in the field of size <span class="tex-span"><i>n</i> × <i>n</i></span> cells. The field contains <span class="tex-span"><i>m</i></span> apple trees, the <span class="tex-span"><i>i</i></span>-th apple tree is at the cell with coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. Vanya moves towards vector <span class="tex-span">(<i>dx</i>, <i>dy</i>)</span>. That means that if Vanya is now at the cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, then in a second he will be at cell <img align="middle" class="tex-formula" src="file://FzEoCRWR.png" style="max-width: 100.0%;max-height: 100.0%;">. The following condition is satisfied for the vector: <img align="middle" class="tex-formula" src="file://LMiPuCUs.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://6SREPVVA.png" style="max-width: 100.0%;max-height: 100.0%;"> is the largest integer that divides both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Vanya ends his path when he reaches the square he has already visited. </p><p>Vanya wonders, from what square of the field he should start his path to see as many apple trees as possible.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>dx</i>, <i>dy</i></span>(<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>dx</i>, <i>dy</i> ≤ <i>n</i></span>) — the size of the field, the number of apple trees and the vector of Vanya's movement. Next <span class="tex-span"><i>m</i></span> lines contain integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the coordinates of apples. One cell may contain multiple apple trees.</p></div><div class="output-specification"><p>Print two space-separated numbers — the coordinates of the cell from which you should start your path. <span class="tex-font-style-bf">If there are several answers you are allowed to print any of them</span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>dx</i>, <i>dy</i></span>(<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>dx</i>, <i>dy</i> ≤ <i>n</i></span>) — the size of the field, the number of apple trees and the vector of Vanya's movement. Next <span class="tex-span"><i>m</i></span> lines contain integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>) — the coordinates of apples. One cell may contain multiple apple trees.</p>

## Output

<p>Print two space-separated numbers — the coordinates of the cell from which you should start your path. <span class="tex-font-style-bf">If there are several answers you are allowed to print any of them</span>.</p>





```input1
5 5 2 3
0 0
1 2
1 3
2 4
3 1

```




```input2
2 3 1 1
0 0
0 1
1 1

```




```output1
1 3

```




```output2
0 0

```



## Note

<p>In the first sample Vanya's path will look like: <span class="tex-span">(1, 3) - (3, 1) - (0, 4) - (2, 2) - (4, 0) - (1, 3)</span></p><p>In the second sample: <span class="tex-span">(0, 0) - (1, 1) - (0, 0)</span></p>
