## Description

<div><p>You have written on a piece of paper an array of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> and <span class="tex-span"><i>m</i></span> <span class="tex-font-style-it">good</span> pairs of integers <span class="tex-span">(<i>i</i><sub class="lower-index">1</sub>, <i>j</i><sub class="lower-index">1</sub>), (<i>i</i><sub class="lower-index">2</sub>, <i>j</i><sub class="lower-index">2</sub>), ..., (<i>i</i><sub class="lower-index"><i>m</i></sub>, <i>j</i><sub class="lower-index"><i>m</i></sub>)</span>. Each <span class="tex-font-style-it">good</span> pair <span class="tex-span">(<i>i</i><sub class="lower-index"><i>k</i></sub>, <i>j</i><sub class="lower-index"><i>k</i></sub>)</span> meets the following conditions: <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub> + <i>j</i><sub class="lower-index"><i>k</i></sub></span> is an odd number and <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index"><i>k</i></sub> &lt; <i>j</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>.</p><p>In one operation you can perform a sequence of actions: </p><ul> <li> take one of the <span class="tex-font-style-it">good</span> pairs <span class="tex-span">(<i>i</i><sub class="lower-index"><i>k</i></sub>, <i>j</i><sub class="lower-index"><i>k</i></sub>)</span> and some integer <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>v</i> &gt; 1</span>), which divides both numbers <span class="tex-span"><i>a</i>[<i>i</i><sub class="lower-index"><i>k</i></sub>]</span> and <span class="tex-span"><i>a</i>[<i>j</i><sub class="lower-index"><i>k</i></sub>]</span>; </li><li> divide both numbers by <span class="tex-span"><i>v</i></span>, i. e. perform the assignments: <img align="middle" class="tex-formula" src="file://mTcUxzfw.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://V927KfBw.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>Determine the maximum number of operations you can sequentially perform on the given array. Note that one pair may be used several times in the described operations.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>) — the description of the array.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the description of <span class="tex-font-style-it">good</span> pairs. The <span class="tex-span"><i>k</i></span>-th line contains two space-separated integers <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>j</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index"><i>k</i></sub> &lt; <i>j</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub> + <i>j</i><sub class="lower-index"><i>k</i></sub></span> is an odd number).</p><p>It is guaranteed that all the <span class="tex-font-style-it">good</span> pairs are distinct.</p></div><div class="output-specification"><p>Output the answer for the problem.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">9</sup></span>) — the description of the array.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the description of <span class="tex-font-style-it">good</span> pairs. The <span class="tex-span"><i>k</i></span>-th line contains two space-separated integers <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub></span>, <span class="tex-span"><i>j</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i><sub class="lower-index"><i>k</i></sub> &lt; <i>j</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i><sub class="lower-index"><i>k</i></sub> + <i>j</i><sub class="lower-index"><i>k</i></sub></span> is an odd number).</p><p>It is guaranteed that all the <span class="tex-font-style-it">good</span> pairs are distinct.</p>

## Output

<p>Output the answer for the problem.</p>





```input1
3 2
8 3 8
1 2
2 3

```




```input2
3 2
8 12 8
1 2
2 3

```




```output1
0

```




```output2
2

```


