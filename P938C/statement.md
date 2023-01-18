## Description

<div><p>Let's denote a <span class="tex-span"><i>m</i></span>-free matrix as a binary (that is, consisting of only <span class="tex-span">1</span>'s and <span class="tex-span">0</span>'s) matrix such that every square submatrix of size <span class="tex-span"><i>m</i> × <i>m</i></span> of this matrix contains at least one zero. </p><p>Consider the following problem:</p><p><span class="tex-font-style-it">You are given two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>. You have to construct an <span class="tex-span"><i>m</i></span>-free square matrix of size <span class="tex-span"><i>n</i> × <i>n</i></span> such that <span class="tex-font-style-bf">the number of <span class="tex-span">1</span>'s in this matrix is maximum possible</span>. Print the maximum possible number of <span class="tex-span">1</span>'s in such matrix.</span></p><p>You don't have to solve this problem. Instead, you have to construct a few tests for it.</p><p>You will be given <span class="tex-span"><i>t</i></span> numbers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>x</i><sub class="lower-index"><i>t</i></sub></span>. For every <img align="middle" class="tex-formula" src="file://1gPvaYWK.png" style="max-width: 100.0%;max-height: 100.0%;">, find two integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> ≥ <i>m</i><sub class="lower-index"><i>i</i></sub></span>) such that the answer for the aforementioned problem is exactly <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> if we set <span class="tex-span"><i>n</i> = <i>n</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i> = <i>m</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>) — the number of tests you have to construct.</p><p>Then <span class="tex-span"><i>t</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p><span class="tex-font-style-bf">Note that in hacks you have to set <span class="tex-span"><i>t</i> = 1</span></span>.</p></div><div class="output-specification"><p>For each test you have to construct, output two positive numbers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) such that the maximum number of <span class="tex-span">1</span>'s in a <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>-free <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> × <i>n</i><sub class="lower-index"><i>i</i></sub></span> matrix is exactly <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. If there are multiple solutions, you may output any of them; and if this is impossible to construct a test, output a single integer <span class="tex-span"> - 1</span>. </p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100</span>) — the number of tests you have to construct.</p><p>Then <span class="tex-span"><i>t</i></span> lines follow, <span class="tex-span"><i>i</i></span>-th line containing one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p><span class="tex-font-style-bf">Note that in hacks you have to set <span class="tex-span"><i>t</i> = 1</span></span>.</p>

## Output

<p>For each test you have to construct, output two positive numbers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) such that the maximum number of <span class="tex-span">1</span>'s in a <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>-free <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> × <i>n</i><sub class="lower-index"><i>i</i></sub></span> matrix is exactly <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. If there are multiple solutions, you may output any of them; and if this is impossible to construct a test, output a single integer <span class="tex-span"> - 1</span>. </p>





```input1
3
21
0
1

```




```output1
5 2
1 1
-1

```


