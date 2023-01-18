## Description

<div><p>Dima got into number sequences. Now he's got sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> positive integers. Also, Dima has got a function <span class="tex-span"><i>f</i>(<i>x</i>)</span>, which can be defined with the following recurrence:</p><ul> <li> <span class="tex-span"><i>f</i>(0) = 0</span>; </li><li> <span class="tex-span"><i>f</i>(2·<i>x</i>) = <i>f</i>(<i>x</i>)</span>; </li><li> <span class="tex-span"><i>f</i>(2·<i>x</i> + 1) = <i>f</i>(<i>x</i>) + 1</span>. </li></ul><p>Dima wonders, how many pairs of indexes <span class="tex-span">(<i>i</i>, <i>j</i>)</span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i>)</span> are there, such that <span class="tex-span"><i>f</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>) = <i>f</i>(<i>a</i><sub class="lower-index"><i>j</i></sub>)</span>. Help him, count the number of such pairs. </p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In a single line print the answer to the problem.</p><p>Please, don't use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>In a single line print the answer to the problem.</p><p>Please, don't use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in <span class="tex-font-style-it">C++</span>. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
1 2 4

```




```input2
3
5 3 1

```




```output1
3

```




```output2
1

```



## Note

<p>In the first sample any pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> will do, so the answer is <span class="tex-span">3</span>.</p><p>In the second sample only pair <span class="tex-span">(1, 2)</span> will do.</p>
