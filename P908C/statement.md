## Description

<div><p>Carol is currently curling.</p><p>She has <span class="tex-span"><i>n</i></span> disks each with radius <span class="tex-span"><i>r</i></span> on the 2D plane. </p><p>Initially she has all these disks above the line <span class="tex-span"><i>y</i> = 10<sup class="upper-index">100</sup></span>.</p><p>She then will slide the disks towards the line <span class="tex-span"><i>y</i> = 0</span> one by one in order from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p><p>When she slides the <span class="tex-span"><i>i</i></span>-th disk, she will place its center at the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, 10<sup class="upper-index">100</sup>)</span>. She will then push it so the disk’s <span class="tex-span"><i>y</i></span> coordinate continuously decreases, and <span class="tex-span"><i>x</i></span> coordinate stays constant. The disk stops once it touches the line <span class="tex-span"><i>y</i> = 0</span> or it touches any previous disk. Note that once a disk stops moving, it will not move again, even if hit by another disk. </p><p>Compute the <span class="tex-span"><i>y</i></span>-coordinates of centers of all the disks after all disks have been pushed.</p></div><div class="input-specification"><p>The first line will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>r</i> ≤ 1 000</span>), the number of disks, and the radius of the disks, respectively.</p><p>The next line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000</span>)&nbsp;— the <span class="tex-span"><i>x</i></span>-coordinates of the disks.</p></div><div class="output-specification"><p>Print a single line with <span class="tex-span"><i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th number denotes the <span class="tex-span"><i>y</i></span>-coordinate of the center of the <span class="tex-span"><i>i</i></span>-th disk. The output will be accepted if it has absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely, let's assume that your answer for a particular value of a coordinate is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://551s80FM.png" style="max-width: 100.0%;max-height: 100.0%;"> for all coordinates.</p></div>

## Input

<p>The first line will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>r</i> ≤ 1 000</span>), the number of disks, and the radius of the disks, respectively.</p><p>The next line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000</span>)&nbsp;— the <span class="tex-span"><i>x</i></span>-coordinates of the disks.</p>

## Output

<p>Print a single line with <span class="tex-span"><i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th number denotes the <span class="tex-span"><i>y</i></span>-coordinate of the center of the <span class="tex-span"><i>i</i></span>-th disk. The output will be accepted if it has absolute or relative error at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely, let's assume that your answer for a particular value of a coordinate is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://551s80FM.png" style="max-width: 100.0%;max-height: 100.0%;"> for all coordinates.</p>





```input1
6 2
5 5 6 8 3 12

```




```output1
2 6.0 9.87298334621 13.3370849613 12.5187346573 13.3370849613

```



## Note

<p>The final positions of the disks will look as follows:</p><center> <img class="tex-graphics" src="file://SiYYjREi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In particular, note the position of the last disk. </p>
