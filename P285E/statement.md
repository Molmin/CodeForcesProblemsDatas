## Description

<div><p><span class="tex-font-style-it"><span class="tex-font-style-bf">Permutation</span> <span class="tex-span"><i>p</i></span> is an ordered set of integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> distinct positive integers, each of them doesn't exceed <span class="tex-span"><i>n</i></span>. We'll denote the <span class="tex-span"><i>i</i></span>-th element of permutation <span class="tex-span"><i>p</i></span> as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. We'll call number <span class="tex-span"><i>n</i></span> the size or the length of permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span>.</span></p><p>We'll call position <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) in permutation <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-font-style-it">good</span>, if <span class="tex-span">|<i>p</i>[<i>i</i>] - <i>i</i>| = 1</span>. Count the number of permutations of size <span class="tex-span"><i>n</i></span> with exactly <span class="tex-span"><i>k</i></span> good positions. Print the answer modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The single line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>k</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the number of permutations of length <span class="tex-span"><i>n</i></span> with exactly <span class="tex-span"><i>k</i></span> good positions modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The single line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>k</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print the number of permutations of length <span class="tex-span"><i>n</i></span> with exactly <span class="tex-span"><i>k</i></span> good positions modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
1 0

```




```input2
2 1

```




```input3
3 2

```




```input4
4 1

```




```input5
7 4

```




```output1
1

```




```output2
0

```




```output3
4

```




```output4
6

```




```output5
328

```



## Note

<p>The only permutation of size 1 has 0 good positions.</p><p>Permutation <span class="tex-span">(1, 2)</span> has 0 good positions, and permutation <span class="tex-span">(2, 1)</span> has 2 positions.</p><p>Permutations of size 3:</p><ol><li> <span class="tex-span">(1, 2, 3)</span> — 0 positions</li><li> <img align="middle" class="tex-formula" src="file://h65zxwZF.png" style="max-width: 100.0%;max-height: 100.0%;"> — 2 positions</li><li> <img align="middle" class="tex-formula" src="file://51AIQLwc.png" style="max-width: 100.0%;max-height: 100.0%;"> — 2 positions</li><li> <img align="middle" class="tex-formula" src="file://8WfSF3JF.png" style="max-width: 100.0%;max-height: 100.0%;"> — 2 positions</li><li> <img align="middle" class="tex-formula" src="file://LOcHUwOD.png" style="max-width: 100.0%;max-height: 100.0%;"> — 2 positions</li><li> <span class="tex-span">(3, 2, 1)</span> — 0 positions</li></ol>
