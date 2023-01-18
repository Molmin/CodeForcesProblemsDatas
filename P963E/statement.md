## Description

<div><p>A chip was placed on a field with coordinate system onto point <span class="tex-span">(0, 0)</span>.</p><p>Every second the chip moves randomly. If the chip is currently at a point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, after a second it moves to the point <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span> with probability <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, to the point <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span> with probability <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span>, to the point <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span> with probability <span class="tex-span"><i>p</i><sub class="lower-index">3</sub></span> and to the point <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span> with probability <span class="tex-span"><i>p</i><sub class="lower-index">4</sub></span>. It's guaranteed that <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> + <i>p</i><sub class="lower-index">2</sub> + <i>p</i><sub class="lower-index">3</sub> + <i>p</i><sub class="lower-index">4</sub> = 1</span>. The moves are independent.</p><p>Find out the expected time after which chip will move away from origin at a distance greater than <span class="tex-span"><i>R</i></span> (i.e. <img align="middle" class="tex-formula" src="file://kMWeIUBK.png" style="max-width: 100.0%;max-height: 100.0%;"> will be satisfied).</p></div><div class="input-specification"><p>First line contains five integers <span class="tex-span"><i>R</i>, <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">0 ≤ <i>R</i> ≤ 50, 1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub> ≤ 1000</span>).</p><p>Probabilities <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> can be calculated using formula <img align="middle" class="tex-formula" src="file://OFpYlaTY.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>It can be shown that answer for this problem is always a rational number of form <img align="middle" class="tex-formula" src="file://Gs9Q9anA.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://Qo4EEndD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Print <span class="tex-span"><i>P</i>·<i>Q</i><sup class="upper-index"> - 1</sup></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p></div>

## Input

<p>First line contains five integers <span class="tex-span"><i>R</i>, <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span> (<span class="tex-span">0 ≤ <i>R</i> ≤ 50, 1 ≤ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub> ≤ 1000</span>).</p><p>Probabilities <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> can be calculated using formula <img align="middle" class="tex-formula" src="file://OFpYlaTY.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>It can be shown that answer for this problem is always a rational number of form <img align="middle" class="tex-formula" src="file://Gs9Q9anA.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://Qo4EEndD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Print <span class="tex-span"><i>P</i>·<i>Q</i><sup class="upper-index"> - 1</sup></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </p>





```input1
0 1 1 1 1

```




```input2
1 1 1 1 1

```




```input3
1 1 2 1 2

```




```output1
1
```




```output2
666666674
```




```output3
538461545
```



## Note

<p>In the first example initially the chip is located at a distance <span class="tex-span">0</span> from origin. In one second chip will move to distance <span class="tex-span">1</span> is some direction, so distance to origin will become <span class="tex-span">1</span>.</p><p>Answers to the second and the third tests: <img align="middle" class="tex-formula" src="file://b1LqKloS.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://F9FxJOrK.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
