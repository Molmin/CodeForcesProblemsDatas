## Description

<div><p>You have an array of positive integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> and a set of <span class="tex-font-style-it">bad</span> prime numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. The prime numbers that do not occur in the set <span class="tex-span"><i>b</i></span> are considered <span class="tex-font-style-it">good</span>. The <span class="tex-font-style-it">beauty</span> of array <span class="tex-span"><i>a</i></span> is the sum <img align="middle" class="tex-formula" src="file://kECgp0u6.png" style="max-width: 100.0%;max-height: 100.0%;">, where function <span class="tex-span"><i>f</i>(<i>s</i>)</span> is determined as follows:</p><ul> <li> <span class="tex-span"><i>f</i>(1) = 0</span>; </li><li> Let's assume that <span class="tex-span"><i>p</i></span> is the minimum prime divisor of <span class="tex-span"><i>s</i></span>. If <span class="tex-span"><i>p</i></span> is a good prime, then <img align="middle" class="tex-formula" src="file://bpnuGN5h.png" style="max-width: 100.0%;max-height: 100.0%;">, otherwise <img align="middle" class="tex-formula" src="file://MPK72TGk.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>You are allowed to perform an arbitrary (probably zero) number of operations to improve array <span class="tex-span"><i>a</i></span>. The <span class="tex-font-style-it">operation of improvement</span> is the following sequence of actions:</p><ul> <li> Choose some number <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span>) and calculate the value <span class="tex-span"><i>g</i></span> = GCD(<span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>r</i>]</span>). </li><li> Apply the assignments: <img align="middle" class="tex-formula" src="file://IqmuYWZu.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://dD7EILqy.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">...</span>, <img align="middle" class="tex-formula" src="file://5ds1viLl.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>What is the maximum beauty of the array you can get? </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>) showing how many numbers are in the array and how many bad prime numbers there are.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>) — array <span class="tex-span"><i>a</i></span>. The third line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">2 ≤ <i>b</i><sub class="lower-index">1</sub> &lt; <i>b</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>b</i><sub class="lower-index"><i>m</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the set of bad prime numbers.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 5000</span>) showing how many numbers are in the array and how many bad prime numbers there are.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>) — array <span class="tex-span"><i>a</i></span>. The third line contains <span class="tex-span"><i>m</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">2 ≤ <i>b</i><sub class="lower-index">1</sub> &lt; <i>b</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>b</i><sub class="lower-index"><i>m</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the set of bad prime numbers.</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
5 2
4 20 34 10 10
2 5

```




```input2
4 5
2 4 8 16
3 5 7 11 17

```




```output1
-2

```




```output2
10

```



## Note

<p>Note that the answer to the problem can be negative.</p><p>The GCD(<span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span>) is the maximum positive integer that divides each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p>
