## Description

<div><p><span class="tex-font-style-it">DZY loves Fast Fourier Transformation, and he enjoys using it.</span></p><p>Fast Fourier Transformation is an algorithm used to calculate convolution. Specifically, if <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> are sequences with length <span class="tex-span"><i>n</i></span>, which are indexed from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, and</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://xdsNJrS9.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>We can calculate <span class="tex-span"><i>c</i></span> fast using Fast Fourier Transformation.</p><p>DZY made a little change on this formula. Now</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://vXDU4PlJ.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>To make things easier, <span class="tex-span"><i>a</i></span> is a permutation of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and <span class="tex-span"><i>b</i></span> is a sequence only containing <span class="tex-span">0</span> and <span class="tex-span">1</span>. Given <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, DZY needs your help to calculate <span class="tex-span"><i>c</i></span>.</p><p>Because he is naughty, DZY provides a special way to get <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. What you need is only three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>x</i></span>. After getting them, use the code below to generate <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><pre class="verbatim"><br>//x is 64-bit variable;<br>function getNextX() {<br>    x = (x * 37 + 10007) % 1000000007;<br>    return x;<br>}<br>function initAB() {<br>    for(i = 0; i &lt; n; i = i + 1){<br>        a[i] = i + 1;<br>    }<br>    for(i = 0; i &lt; n; i = i + 1){<br>        swap(a[i], a[getNextX() % (i + 1)]);<br>    }<br>    for(i = 0; i &lt; n; i = i + 1){<br>        if (i &lt; d)<br>            b[i] = 1;<br>        else<br>            b[i] = 0;<br>    }<br>    for(i = 0; i &lt; n; i = i + 1){<br>        swap(b[i], b[getNextX() % (i + 1)]);<br>    }<br>}<br><br></pre><p>Operation <span class="tex-font-style-tt">x % y</span> denotes remainder after division <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>y</i></span>. Function <span class="tex-font-style-tt">swap(x, y)</span> swaps two values <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p></div><div class="input-specification"><p>The only line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>d</i>, <i>x</i>&nbsp;(1 ≤ <i>d</i> ≤ <i>n</i> ≤ 100000;&nbsp;0 ≤ <i>x</i> ≤ 1000000006)</span>. Because DZY is naughty, <span class="tex-span"><i>x</i></span> can't be equal to <span class="tex-span">27777500</span>.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> - 1</sub></span>.</p></div>

## Input

<p>The only line of input contains three space-separated integers <span class="tex-span"><i>n</i>, <i>d</i>, <i>x</i>&nbsp;(1 ≤ <i>d</i> ≤ <i>n</i> ≤ 100000;&nbsp;0 ≤ <i>x</i> ≤ 1000000006)</span>. Because DZY is naughty, <span class="tex-span"><i>x</i></span> can't be equal to <span class="tex-span">27777500</span>.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line should contain an integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> - 1</sub></span>.</p>





```input1
3 1 1

```




```input2
5 4 2

```




```input3
5 4 3

```




```output1
1
3
2

```




```output2
2
2
4
5
5

```




```output3
5
5
5
5
4

```



## Note

<p>In the first sample, <span class="tex-span"><i>a</i></span> is <span class="tex-span">[1 3 2]</span>, <span class="tex-span"><i>b</i></span> is <span class="tex-span">[1 0 0]</span>, so <span class="tex-span"><i>c</i><sub class="lower-index">0</sub> = <i>max</i>(1·1) = 1</span>, <span class="tex-span"><i>c</i><sub class="lower-index">1</sub> = <i>max</i>(1·0, 3·1) = 3</span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub> = <i>max</i>(1·0, 3·0, 2·1) = 2</span>.</p><p>In the second sample, <span class="tex-span"><i>a</i></span> is <span class="tex-span">[2 1 4 5 3]</span>, <span class="tex-span"><i>b</i></span> is <span class="tex-span">[1 1 1 0 1]</span>.</p><p>In the third sample, <span class="tex-span"><i>a</i></span> is <span class="tex-span">[5 2 1 4 3]</span>, <span class="tex-span"><i>b</i></span> is <span class="tex-span">[1 1 1 1 0]</span>.</p>
