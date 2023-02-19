## Description

<div><p>You are given a non-degenerate triangle (a non-degenerate triangle is a triangle with positive area). The vertices of the triangle have coordinates $(x_1, y_1)$, $(x_2, y_2)$ and $(x_3, y_3)$.</p><p>You want to draw a straight line to cut the triangle into <span class="tex-font-style-bf">two non-degenerate triangles</span>. Furthermore, the line you draw should be <span class="tex-font-style-bf">either horizontal or vertical</span>.</p><p>Can you draw the line to meet all the constraints?</p><p>Here are some suitable ways to draw the line:</p><center> <img class="tex-graphics" src="file://WDbRfEcS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>However, these ways to draw the line are not suitable (the first line cuts the triangle into a triangle and a quadrangle; the second line doesn't cut the triangle at all; the third line is neither horizontal nor vertical):</p><center> <img class="tex-graphics" src="file://sdkRUgqN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of four lines. The first of them is empty. The $i$-th of the next three lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 10^8$) — the coordinates of the $i$-th vertex of the triangle.</p><p>Additional constraint on the input: in each test case, the triangle formed by three vertices has positive area (i. e. it is non-degenerate).</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to cut the triangle according to the statement, or <span class="tex-font-style-tt">NO</span> otherwise. You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of four lines. The first of them is empty. The $i$-th of the next three lines contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le 10^8$) — the coordinates of the $i$-th vertex of the triangle.</p><p>Additional constraint on the input: in each test case, the triangle formed by three vertices has positive area (i. e. it is non-degenerate).</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to cut the triangle according to the statement, or <span class="tex-font-style-tt">NO</span> otherwise. You may print each letter in any case (<span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> will all be recognized as positive answer, <span class="tex-font-style-tt">NO</span>, <span class="tex-font-style-tt">no</span> and <span class="tex-font-style-tt">nO</span> will all be recognized as negative answer).</p>





```input1|2,3,4,5,10,11,12,13
4
<br>
4 7
6 8
3 5
<br>
4 5
4 7
6 8
<br>
5 8
1 8
2 5
<br>
3 6
6 6
6 3
```




```output1
YES
YES
YES
NO
```


