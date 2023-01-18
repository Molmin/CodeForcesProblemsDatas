## Description

<div><p>Inna and Dima decided to surprise Sereja. They brought a really huge candy matrix, it's big even for Sereja! Let's number the rows of the giant matrix from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from top to bottom and the columns — from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, from left to right. We'll represent the cell on the intersection of the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column as <span class="tex-span">(<i>i</i>, <i>j</i>)</span>. Just as is expected, some cells of the giant candy matrix contain candies. Overall the matrix has <span class="tex-span"><i>p</i></span> candies: the <span class="tex-span"><i>k</i></span>-th candy is at cell <span class="tex-span">(<i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub>)</span>.</p><p>The time moved closer to dinner and Inna was already going to eat <span class="tex-span"><i>p</i></span> of her favourite sweets from the matrix, when suddenly Sereja (for the reason he didn't share with anyone) rotated the matrix <span class="tex-span"><i>x</i></span> times clockwise by 90 degrees. Then he performed the horizontal rotate of the matrix <span class="tex-span"><i>y</i></span> times. And then he rotated the matrix <span class="tex-span"><i>z</i></span> times counterclockwise by 90 degrees. The figure below shows how the rotates of the matrix looks like.</p><center> <img class="tex-graphics" src="file://TH3TDmsv.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Inna got really upset, but Duma suddenly understood two things: the candies didn't get damaged and he remembered which cells contained Inna's favourite sweets before Sereja's strange actions. Help guys to find the new coordinates in the candy matrix after the transformation Sereja made!</p></div><div class="input-specification"><p>The first line of the input contains fix integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>z</i></span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>p</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the following <span class="tex-span"><i>p</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>k</i></sub> ≤ <i>m</i>)</span> — the initial coordinates of the <span class="tex-span"><i>k</i></span>-th candy. Two candies can lie on the same cell.</p></div><div class="output-specification"><p>For each of the <span class="tex-span"><i>p</i></span> candies, print on a single line its space-separated new coordinates.</p></div>

## Input

<p>The first line of the input contains fix integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>z</i></span>, <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;0 ≤ <i>x</i>, <i>y</i>, <i>z</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>p</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the following <span class="tex-span"><i>p</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>k</i></sub> ≤ <i>m</i>)</span> — the initial coordinates of the <span class="tex-span"><i>k</i></span>-th candy. Two candies can lie on the same cell.</p>

## Output

<p>For each of the <span class="tex-span"><i>p</i></span> candies, print on a single line its space-separated new coordinates.</p>





```input1
3 3 3 1 1 9
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3

```




```output1
1 3
1 2
1 1
2 3
2 2
2 1
3 3
3 2
3 1

```



## Note

<p>Just for clarity. Horizontal rotating is like a mirroring of the matrix. For matrix:</p><pre class="verbatim"><br>QWER      REWQ <br>ASDF  -&gt;  FDSA<br>ZXCV      VCXZ<br></pre>
