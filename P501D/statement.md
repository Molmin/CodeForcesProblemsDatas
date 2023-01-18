## Description

<div><p>Let's define the sum of two permutations <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> of numbers <span class="tex-span">0, 1, ..., (<i>n</i> - 1)</span> as permutation <img align="middle" class="tex-formula" src="file://9FfhtN0a.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>Perm</i>(<i>x</i>)</span> is the <span class="tex-span"><i>x</i></span>-th lexicographically permutation of numbers <span class="tex-span">0, 1, ..., (<i>n</i> - 1)</span> (counting from zero), and <span class="tex-span"><i>Ord</i>(<i>p</i>)</span> is the number of permutation <span class="tex-span"><i>p</i></span> in the lexicographical order.</p><p>For example, <span class="tex-span"><i>Perm</i>(0) = (0, 1, ..., <i>n</i> - 2, <i>n</i> - 1)</span>, <span class="tex-span"><i>Perm</i>(<i>n</i>! - 1) = (<i>n</i> - 1, <i>n</i> - 2, ..., 1, 0)</span></p><p>Misha has two permutations, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>. Your task is to find their sum.</p><p>Permutation <span class="tex-span"><i>a</i> = (<i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub>)</span> is called to be lexicographically smaller than permutation <span class="tex-span"><i>b</i> = (<i>b</i><sub class="lower-index">0</sub>, <i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> - 1</sub>)</span>, if for some <span class="tex-span"><i>k</i></span> following conditions hold: <span class="tex-span"><i>a</i><sub class="lower-index">0</sub> = <i>b</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub> = <i>b</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i> - 1</sub> = <i>b</i><sub class="lower-index"><i>k</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>k</i></sub> &lt; <i>b</i><sub class="lower-index"><i>k</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, separated by a space, forming permutation <span class="tex-span"><i>p</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, separated by spaces, forming permutation <span class="tex-span"><i>q</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, forming the sum of the given permutations. Separate the numbers by spaces.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, separated by a space, forming permutation <span class="tex-span"><i>p</i></span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, separated by spaces, forming permutation <span class="tex-span"><i>q</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>, forming the sum of the given permutations. Separate the numbers by spaces.</p>





```input1
2
0 1
0 1

```




```input2
2
0 1
1 0

```




```input3
3
1 2 0
2 1 0

```




```output1
0 1

```




```output2
1 0

```




```output3
1 0 2

```



## Note

<p>Permutations of numbers from 0 to 1 in the lexicographical order: <span class="tex-span">(0, 1), (1, 0)</span>.</p><p>In the first sample <span class="tex-span"><i>Ord</i>(<i>p</i>) = 0</span> and <span class="tex-span"><i>Ord</i>(<i>q</i>) = 0</span>, so the answer is <img align="middle" class="tex-formula" src="file://B3rrjDZH.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample <span class="tex-span"><i>Ord</i>(<i>p</i>) = 0</span> and <span class="tex-span"><i>Ord</i>(<i>q</i>) = 1</span>, so the answer is <img align="middle" class="tex-formula" src="file://cGIufIKP.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Permutations of numbers from 0 to 2 in the lexicographical order: <span class="tex-span">(0, 1, 2), (0, 2, 1), (1, 0, 2), (1, 2, 0), (2, 0, 1), (2, 1, 0)</span>.</p><p>In the third sample <span class="tex-span"><i>Ord</i>(<i>p</i>) = 3</span> and <span class="tex-span"><i>Ord</i>(<i>q</i>) = 5</span>, so the answer is <img align="middle" class="tex-formula" src="file://7lTqLrWx.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
