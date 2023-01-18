## Description

<div><p>You are given an array <span class="tex-span"><i>s</i></span> of <span class="tex-span"><i>n</i></span> non-negative integers.</p><p>A 5-tuple of integers <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>e</i>)</span> is said to be valid if it satisfies the following conditions: </p><ul> <li> <span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>e</i> ≤ <i>n</i></span> </li><li> <span class="tex-span">(<i>s</i><sub class="lower-index"><i>a</i></sub></span> | <span class="tex-span"><i>s</i><sub class="lower-index"><i>b</i></sub>)</span> &amp; <span class="tex-span"><i>s</i><sub class="lower-index"><i>c</i></sub></span> &amp; <span class="tex-span">(<i>s</i><sub class="lower-index"><i>d</i></sub></span> ^ <span class="tex-span"><i>s</i><sub class="lower-index"><i>e</i></sub>) = 2<sup class="upper-index"><i>i</i></sup></span> for some integer <span class="tex-span"><i>i</i></span> </li><li> <span class="tex-span"><i>s</i><sub class="lower-index"><i>a</i></sub></span> &amp; <span class="tex-span"><i>s</i><sub class="lower-index"><i>b</i></sub> = 0</span> </li></ul><p>Here, '|' is the bitwise OR, '&amp;' is the bitwise AND and '^' is the bitwise XOR operation.</p><p>Find the sum of <span class="tex-span"><i>f</i>(<i>s</i><sub class="lower-index"><i>a</i></sub></span>|<span class="tex-span"><i>s</i><sub class="lower-index"><i>b</i></sub>) * <i>f</i>(<i>s</i><sub class="lower-index"><i>c</i></sub>) * <i>f</i>(<i>s</i><sub class="lower-index"><i>d</i></sub></span>^<span class="tex-span"><i>s</i><sub class="lower-index"><i>e</i></sub>)</span> over all valid 5-tuples <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>e</i>)</span>, where <span class="tex-span"><i>f</i>(<i>i</i>)</span> is the <span class="tex-span"><i>i</i></span>-th Fibonnaci number (<span class="tex-span"><i>f</i>(0) = 0, <i>f</i>(1) = 1, <i>f</i>(<i>i</i>) = <i>f</i>(<i>i</i> - 1) + <i>f</i>(<i>i</i> - 2)</span>).</p><p>Since answer can be is huge output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">17</sup></span>).</p></div><div class="output-specification"><p>Output the sum as described above, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span></p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">17</sup></span>).</p>

## Output

<p>Output the sum as described above, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span></p>





```input1
2
1 2

```




```input2
3
7 4 1

```




```input3
10
1 3 0 7 3 7 6 5 7 5

```




```input4
10
50 9 11 44 39 40 5 39 23 7

```




```output1
32

```




```output2
3520

```




```output3
1235424

```




```output4
113860062

```


