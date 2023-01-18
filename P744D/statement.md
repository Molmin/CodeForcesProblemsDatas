## Description

<div><p>Hongcow really likes the color red. Hongcow doesn't like the color blue.</p><p>Hongcow is standing in an infinite field where there are <span class="tex-span"><i>n</i></span> red points and <span class="tex-span"><i>m</i></span> blue points.</p><p>Hongcow wants to draw a circle in the field such that this circle contains at least one red point, and no blue points. Points that line exactly on the boundary of the circle can be counted as either inside or outside.</p><p>Compute the radius of the largest circle that satisfies this condition. If this circle can have arbitrarily large size, print <span class="tex-span"> - 1</span>. Otherwise, your answer will be accepted if it has relative or absolute error at most <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div><div class="input-specification"><p>The first line of the input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1, 000</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). This denotes the coordinates of a red point.</p><p>The next <span class="tex-span"><i>m</i></span> lines will contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). This denotes the coordinates of a blue point.</p><p>No two points will have the same coordinates.</p></div><div class="output-specification"><p>Print <span class="tex-span"> - 1</span> if the circle can have arbitrary size. Otherwise, print a floating point number representing the largest radius circle that satisfies the conditions. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://O3v8Hw5v.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1, 000</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines will contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). This denotes the coordinates of a red point.</p><p>The next <span class="tex-span"><i>m</i></span> lines will contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). This denotes the coordinates of a blue point.</p><p>No two points will have the same coordinates.</p>

## Output

<p>Print <span class="tex-span"> - 1</span> if the circle can have arbitrary size. Otherwise, print a floating point number representing the largest radius circle that satisfies the conditions. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p><p>Namely, let's assume that your answer is <span class="tex-span"><i>a</i></span> and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://O3v8Hw5v.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 5
2 3
3 4
1 1
1 4
4 2
4 7
2 5

```




```input2
1 6
3 3
1 5
5 4
2 1
3 4
4 2
1 3

```




```input3
2 2
2 2
3 3
1 1
4 4

```




```output1
3.5355338827

```




```output2
1.5811388195

```




```output3
-1

```



## Note

<p>This is a picture of the first sample </p><center> <img class="tex-graphics" src="file://2XpPJ8M5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>This is a picture of the second sample </p><center> <img class="tex-graphics" src="file://4YhVfNIX.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
