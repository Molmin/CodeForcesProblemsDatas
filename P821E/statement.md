## Description

<div><p>Okabe likes to take walks but knows that spies from the Organization could be anywhere; that's why he wants to know how many different walks he can take in his city safely. Okabe's city can be represented as all points <span class="tex-span">(<i>x</i>, <i>y</i>)</span> such that <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are non-negative. Okabe starts at the origin (point <span class="tex-span">(0, 0)</span>), and needs to reach the point <span class="tex-span">(<i>k</i>, 0)</span>. If Okabe is currently at the point <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, in one step he can go to <span class="tex-span">(<i>x</i> + 1, <i>y</i> + 1)</span>, <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>, or <span class="tex-span">(<i>x</i> + 1, <i>y</i> - 1)</span>.</p><p>Additionally, there are <span class="tex-span"><i>n</i></span> horizontal line segments, the <span class="tex-span"><i>i</i></span>-th of which goes from <span class="tex-span"><i>x</i> = <i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>x</i> = <i>b</i><sub class="lower-index"><i>i</i></sub></span> inclusive, and is at <span class="tex-span"><i>y</i> = <i>c</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> ≤ <i>k</i> ≤ <i>b</i><sub class="lower-index"><i>n</i></sub></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i> - 1</sub></span> for <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th line segment forces Okabe to walk with <span class="tex-span"><i>y</i></span>-value in the range <span class="tex-span">0 ≤ <i>y</i> ≤ <i>c</i><sub class="lower-index"><i>i</i></sub></span> when his <span class="tex-span"><i>x</i></span> value satisfies <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, or else he might be spied on. This also means he is required to be under two line segments when one segment ends and another begins.</p><p>Okabe now wants to know how many walks there are from the origin to the point <span class="tex-span">(<i>k</i>, 0)</span> satisfying these conditions, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of input contains the integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of segments and the destination <span class="tex-span"><i>x</i></span> coordinate.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 15</span>)&nbsp;— the left and right ends of a segment, and its <span class="tex-span"><i>y</i></span> coordinate.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> ≤ <i>k</i> ≤ <i>b</i><sub class="lower-index"><i>n</i></sub></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i> - 1</sub></span> for <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>.</p></div><div class="output-specification"><p>Print the number of walks satisfying the conditions, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line of input contains the integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of segments and the destination <span class="tex-span"><i>x</i></span> coordinate.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 15</span>)&nbsp;— the left and right ends of a segment, and its <span class="tex-span"><i>y</i></span> coordinate.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 0</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub> ≤ <i>k</i> ≤ <i>b</i><sub class="lower-index"><i>n</i></sub></span>, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i> - 1</sub></span> for <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>.</p>

## Output

<p>Print the number of walks satisfying the conditions, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
1 3
0 3 3

```




```input2
2 6
0 3 0
3 10 2

```




```output1
4

```




```output2
4

```



## Note

<center> <img class="tex-graphics" src="file://4TktAlog.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The graph above corresponds to sample 1. The possible walks are:</p><ul> <li> <img align="middle" class="tex-formula" src="file://K6lErX1m.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://0lMjJWdC.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://TOu2xqd2.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://LJHJs933.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ul><center> <img class="tex-graphics" src="file://cone2hSx.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The graph above corresponds to sample 2. There is only one walk for Okabe to reach <span class="tex-span">(3, 0)</span>. After this, the possible walks are:</p><ul> <li> <img align="middle" class="tex-formula" src="file://LG0nvEkJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://eSQUJVEe.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://lByve3BD.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> <img align="middle" class="tex-formula" src="file://nTpVatiV.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ul>
