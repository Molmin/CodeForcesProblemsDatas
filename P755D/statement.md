## Description

<div><p>PolandBall has such a convex polygon with <span class="tex-span"><i>n</i></span> veritces that no three of its diagonals intersect at the same point. PolandBall decided to improve it and draw some red segments. </p><p>He chose a number <span class="tex-span"><i>k</i></span> such that <span class="tex-span"><i>gcd</i>(<i>n</i>, <i>k</i>) = 1</span>. Vertices of the polygon are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in a clockwise way. PolandBall repeats the following process <span class="tex-span"><i>n</i></span> times, starting from the vertex <span class="tex-span">1</span>: </p><p><span class="tex-font-style-tt">Assume you've ended last operation in vertex <span class="tex-span"><i>x</i></span> (consider <span class="tex-span"><i>x</i> = 1</span> if it is the first operation). Draw a new segment from vertex <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>k</i></span>-th next vertex in clockwise direction. This is a vertex <span class="tex-span"><i>x</i> + <i>k</i></span> or <span class="tex-span"><i>x</i> + <i>k</i> - <i>n</i></span> depending on which of these is a valid index of polygon's vertex.</span></p><p>Your task is to calculate number of polygon's sections after each drawing. A section is a clear area inside the polygon bounded with drawn diagonals or the polygon's sides.</p></div><div class="input-specification"><p>There are only two numbers in the input: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> - 2</span>, <span class="tex-span"><i>gcd</i>(<i>n</i>, <i>k</i>) = 1</span>).</p></div><div class="output-specification"><p>You should print <span class="tex-span"><i>n</i></span> values separated by spaces. The <span class="tex-span"><i>i</i></span>-th value should represent number of polygon's sections after drawing first <span class="tex-span"><i>i</i></span> lines.</p></div>

## Input

<p>There are only two numbers in the input: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> - 2</span>, <span class="tex-span"><i>gcd</i>(<i>n</i>, <i>k</i>) = 1</span>).</p>

## Output

<p>You should print <span class="tex-span"><i>n</i></span> values separated by spaces. The <span class="tex-span"><i>i</i></span>-th value should represent number of polygon's sections after drawing first <span class="tex-span"><i>i</i></span> lines.</p>





```input1
5 2

```




```input2
10 3

```




```output1
2 3 5 8 11
```




```output2
2 3 4 6 9 12 16 21 26 31
```



## Note

<p>The greatest common divisor (gcd) of two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is the largest positive integer that divides both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> without a remainder.</p><p>For the first sample testcase, you should output "<span class="tex-font-style-tt">2 3 5 8 11</span>". Pictures below correspond to situations after drawing lines.</p><center> <img class="tex-graphics" src="file://2lwBbetl.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://x82tdcAe.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://Rn4Vrn2q.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://nrFaPMsp.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://u8LnYVh4.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://ailR23GK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
