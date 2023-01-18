## Description

<div><p><span class="tex-font-style-it"><span class="tex-font-style-bf">Permutation</span> <span class="tex-span"><i>p</i></span> is an ordered set of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers, each of them doesn't exceed <span class="tex-span"><i>n</i></span>. We'll denote the <span class="tex-span"><i>i</i></span>-th element of permutation <span class="tex-span"><i>p</i></span> as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. We'll call number <span class="tex-span"><i>n</i></span> the size or the length of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>.</span></p><p>Petya decided to introduce the sum operation on the set of permutations of length <span class="tex-span"><i>n</i></span>. Let's assume that we are given two permutations of length <span class="tex-span"><i>n</i></span>: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. Petya calls the sum of permutations <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> such permutation <span class="tex-span"><i>c</i></span> of length <span class="tex-span"><i>n</i></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = ((<i>a</i><sub class="lower-index"><i>i</i></sub> - 1 + <i>b</i><sub class="lower-index"><i>i</i></sub> - 1) <i>mod</i> <i>n</i>) + 1</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>.</p><p>Operation <img align="middle" class="tex-formula" src="file://WmAUtdJA.png" style="max-width: 100.0%;max-height: 100.0%;"> means taking the remainder after dividing number <span class="tex-span"><i>x</i></span> by number <span class="tex-span"><i>y</i></span>.</p><p>Obviously, not for all permutations <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> exists permutation <span class="tex-span"><i>c</i></span> that is sum of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. That's why Petya got sad and asked you to do the following: given <span class="tex-span"><i>n</i></span>, count the number of such pairs of permutations <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>n</i></span>, that exists permutation <span class="tex-span"><i>c</i></span> that is sum of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. The pair of permutations <span class="tex-span"><i>x</i>, <i>y</i></span> <span class="tex-span">(<i>x</i> ≠ <i>y</i>)</span> and the pair of permutations <span class="tex-span"><i>y</i>, <i>x</i></span> are considered distinct pairs.</p><p>As the answer can be rather large, print the remainder after dividing it by <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The single line contains integer <span class="tex-span"><i>n</i> (1 ≤ <i>n</i> ≤ 16)</span>.</p></div><div class="output-specification"><p>In the single line print a single non-negative integer — the number of such pairs of permutations <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, that exists permutation <span class="tex-span"><i>c</i></span> that is sum of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The single line contains integer <span class="tex-span"><i>n</i> (1 ≤ <i>n</i> ≤ 16)</span>.</p>

## Output

<p>In the single line print a single non-negative integer — the number of such pairs of permutations <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, that exists permutation <span class="tex-span"><i>c</i></span> that is sum of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
3

```




```input2
5

```




```output1
18

```




```output2
1800

```


