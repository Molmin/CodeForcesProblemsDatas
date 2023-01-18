## Description

<div><p>Fafa has an array <span class="tex-span"><i>A</i></span> of <span class="tex-span"><i>n</i></span> positive integers, the function <span class="tex-span"><i>f</i>(<i>A</i>)</span> is defined as <img align="middle" class="tex-formula" src="file://SOjakkka.png" style="max-width: 100.0%;max-height: 100.0%;">. He wants to do <span class="tex-span"><i>q</i></span> queries of two types:</p><ul> <li> <span class="tex-span">1 <i>l</i> <i>r</i> <i>x</i></span> — find the maximum possible value of <span class="tex-span"><i>f</i>(<i>A</i>)</span>, if <span class="tex-span"><i>x</i></span> is to be added to one element in the range <span class="tex-span">[<i>l</i>,  <i>r</i>]</span>. You can choose to which element to add <span class="tex-span"><i>x</i></span>. </li><li> <span class="tex-span">2 <i>l</i> <i>r</i> <i>x</i></span> — increase all the elements in the range <span class="tex-span">[<i>l</i>,  <i>r</i>]</span> by value <span class="tex-span"><i>x</i></span>. </li></ul><p>Note that queries of type <span class="tex-span">1</span> don't affect the array elements.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the length of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 &lt; <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the array elements.</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. </p><p>Then <span class="tex-span"><i>q</i></span> lines follow, line <span class="tex-span"><i>i</i></span> describes the <span class="tex-span"><i>i</i></span>-th query and contains four integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> <i>l</i><sub class="lower-index"><i>i</i></sub> <i>r</i><sub class="lower-index"><i>i</i></sub> <i>x</i><sub class="lower-index"><i>i</i></sub></span> <img align="middle" class="tex-formula" src="file://Z2adl8MR.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>It is guaranteed that at least one of the queries is of type <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>For each query of type <span class="tex-span">1</span>, print the answer to the query.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the length of the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 &lt; <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the array elements.</p><p>The third line contains an integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of queries. </p><p>Then <span class="tex-span"><i>q</i></span> lines follow, line <span class="tex-span"><i>i</i></span> describes the <span class="tex-span"><i>i</i></span>-th query and contains four integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> <i>l</i><sub class="lower-index"><i>i</i></sub> <i>r</i><sub class="lower-index"><i>i</i></sub> <i>x</i><sub class="lower-index"><i>i</i></sub></span> <img align="middle" class="tex-formula" src="file://Z2adl8MR.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>It is guaranteed that at least one of the queries is of type <span class="tex-span">1</span>.</p>

## Output

<p>For each query of type <span class="tex-span">1</span>, print the answer to the query.</p>





```input1
5
1 1 1 1 1
5
1 2 4 1
2 2 3 1
2 4 4 2
2 3 4 1
1 3 3 2

```




```input2
5
1 2 3 4 5
4
1 2 4 2
2 2 4 1
2 3 4 1
1 2 4 2

```




```output1
2
8

```




```output2
6
10

```


