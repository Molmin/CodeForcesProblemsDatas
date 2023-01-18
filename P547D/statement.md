## Description

<div><p>As everyone knows, bears love fish. But Mike is a strange bear; He hates fish! The even more strange thing about him is he has an infinite number of blue and red fish. </p><center> <img class="tex-graphics" src="file://WtbbkWNC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>He has marked <span class="tex-span"><i>n</i></span> distinct points in the plane. <span class="tex-span"><i>i</i></span>-th point is point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. He wants to put exactly one fish in each of these points such that the difference between the number of red fish and the blue fish on each horizontal or vertical line is at most 1.</p><p>He can't find a way to perform that! Please help him.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the information about the points, <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 2 × 10<sup class="upper-index">5</sup></span>), the <span class="tex-span"><i>i</i></span>-th point coordinates.</p><p>It is guaranteed that there is at least one valid answer.</p></div><div class="output-specification"><p>Print the answer as a sequence of <span class="tex-span"><i>n</i></span> characters 'r' (for red) or 'b' (for blue) where <span class="tex-span"><i>i</i></span>-th character denotes the color of the fish in the <span class="tex-span"><i>i</i></span>-th point.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the information about the points, <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 2 × 10<sup class="upper-index">5</sup></span>), the <span class="tex-span"><i>i</i></span>-th point coordinates.</p><p>It is guaranteed that there is at least one valid answer.</p>

## Output

<p>Print the answer as a sequence of <span class="tex-span"><i>n</i></span> characters 'r' (for red) or 'b' (for blue) where <span class="tex-span"><i>i</i></span>-th character denotes the color of the fish in the <span class="tex-span"><i>i</i></span>-th point.</p>





```input1
4
1 1
1 2
2 1
2 2

```




```input2
3
1 1
1 2
2 1

```




```output1
brrb

```




```output2
brr

```


