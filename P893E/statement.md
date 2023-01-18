## Description

<div><p>You are given two positive integer numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. An array <span class="tex-span"><i>F</i></span> is called an <span class="tex-font-style-it"><span class="tex-span"><i>y</i></span>-factorization</span> of <span class="tex-span"><i>x</i></span> iff the following conditions are met:</p><ul> <li> There are <span class="tex-span"><i>y</i></span> elements in <span class="tex-span"><i>F</i></span>, and all of them are integer numbers; </li><li> <img align="middle" class="tex-formula" src="file://TXASFWVM.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>You have to count the number of pairwise distinct arrays that are <span class="tex-span"><i>y</i></span>-factorizations of <span class="tex-span"><i>x</i></span>. Two arrays <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> are considered different iff there exists at least one index <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>y</i></span>) such that <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub> ≠ <i>B</i><sub class="lower-index"><i>i</i></sub></span>. Since the answer can be very large, print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of testcases to solve.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). Each of these lines represents a testcase.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> integers. <span class="tex-span"><i>i</i></span>-th integer has to be equal to the number of <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-factorizations of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of testcases to solve.</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). Each of these lines represents a testcase.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> integers. <span class="tex-span"><i>i</i></span>-th integer has to be equal to the number of <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>-factorizations of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2
6 3
4 2

```




```output1
36
6

```



## Note

<p>In the second testcase of the example there are six <span class="tex-span"><i>y</i></span>-factorizations:</p><ul> <li> <span class="tex-span">{ - 4,  - 1}</span>; </li><li> <span class="tex-span">{ - 2,  - 2}</span>; </li><li> <span class="tex-span">{ - 1,  - 4}</span>; </li><li> <span class="tex-span">{1, 4}</span>; </li><li> <span class="tex-span">{2, 2}</span>; </li><li> <span class="tex-span">{4, 1}</span>. </li></ul>
