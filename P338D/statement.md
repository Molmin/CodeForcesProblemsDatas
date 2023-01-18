## Description

<div><p>Consider a table <span class="tex-span"><i>G</i></span> of size <span class="tex-span"><i>n</i> × <i>m</i></span> such that <span class="tex-span"><i>G</i>(<i>i</i>, <i>j</i>) = <i>GCD</i>(<i>i</i>, <i>j</i>)</span> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i>, 1 ≤ <i>j</i> ≤ <i>m</i></span>. <span class="tex-span"><i>GCD</i>(<i>a</i>, <i>b</i>)</span> is the greatest common divisor of numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>You have a sequence of positive integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>. We say that this sequence occurs in table <span class="tex-span"><i>G</i></span> if it coincides with consecutive elements in some row, starting from some position. More formally, such numbers <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i> - <i>k</i> + 1</span> should exist that <span class="tex-span"><i>G</i>(<i>i</i>, <i>j</i> + <i>l</i> - 1) = <i>a</i><sub class="lower-index"><i>l</i></sub></span> for all <span class="tex-span">1 ≤ <i>l</i> ≤ <i>k</i></span>.</p><p>Determine if the sequence <span class="tex-span"><i>a</i></span> occurs in table <span class="tex-span"><i>G</i></span>.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">12</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 10000</span>). The second line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p></div><div class="output-specification"><p>Print a single word "<span class="tex-font-style-tt">YES</span>", if the given sequence occurs in table <span class="tex-span"><i>G</i></span>, otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">12</sup></span>; <span class="tex-span">1 ≤ <i>k</i> ≤ 10000</span>). The second line contains <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>).</p>

## Output

<p>Print a single word "<span class="tex-font-style-tt">YES</span>", if the given sequence occurs in table <span class="tex-span"><i>G</i></span>, otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
100 100 5
5 2 1 2 1

```




```input2
100 8 5
5 2 1 2 1

```




```input3
100 100 7
1 2 3 4 5 6 7

```




```output1
YES

```




```output2
NO

```




```output3
NO

```



## Note

<p>Sample 1. The tenth row of table <span class="tex-span"><i>G</i></span> starts from sequence {1, 2, 1, 2, 5, 2, 1, 2, 1, 10}. As you can see, elements from fifth to ninth coincide with sequence <span class="tex-span"><i>a</i></span>.</p><p>Sample 2. This time the width of table <span class="tex-span"><i>G</i></span> equals 8. Sequence <span class="tex-span"><i>a</i></span> doesn't occur there.</p>
