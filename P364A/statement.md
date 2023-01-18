## Description

<div><p>You have a string of decimal digits <span class="tex-span"><i>s</i></span>. Let's define <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub> = <i>s</i><sub class="lower-index"><i>i</i></sub>·<i>s</i><sub class="lower-index"><i>j</i></sub></span>. Find in matrix <span class="tex-span"><i>b</i></span> the number of such rectangles that the sum <span class="tex-span"><i>b</i><sub class="lower-index"><i>ij</i></sub></span> for all cells <span class="tex-span">(<i>i</i>, <i>j</i>)</span> that are the elements of the rectangle equals <span class="tex-span"><i>a</i></span> in each rectangle.</p><p>A rectangle in a matrix is a group of four integers <span class="tex-span">(<i>x</i>, <i>y</i>, <i>z</i>, <i>t</i>)</span> <span class="tex-font-style-bf"><span class="tex-span">(<i>x</i> ≤ <i>y</i>, <i>z</i> ≤ <i>t</i>)</span></span>. The elements of the rectangle are all cells <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span"><i>x</i> ≤ <i>i</i> ≤ <i>y</i>, <i>z</i> ≤ <i>j</i> ≤ <i>t</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>), the second line contains a string of decimal integers <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 4000</span>).</p></div><div class="output-specification"><p>Print a single integer — the answer to a problem.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">0 ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>), the second line contains a string of decimal integers <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 4000</span>).</p>

## Output

<p>Print a single integer — the answer to a problem.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
10
12345

```




```input2
16
439873893693495623498263984765

```




```output1
6

```




```output2
40

```


