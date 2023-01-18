## Description

<div><p>John Doe has found the beautiful permutation formula.</p><p>Let's take permutation <span class="tex-span"><i>p</i> = <i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. Let's define transformation <span class="tex-span"><i>f</i></span> of this permutation: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://zGgBZMaq.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>where <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 1)</span> is an integer, the transformation parameter, <span class="tex-span"><i>r</i></span> is such maximum integer that <span class="tex-span"><i>rk</i> ≤ <i>n</i></span>. If <span class="tex-span"><i>rk</i> = <i>n</i></span>, then elements <span class="tex-span"><i>p</i><sub class="lower-index"><i>rk</i> + 1</sub>, <i>p</i><sub class="lower-index"><i>rk</i> + 2</sub></span> and so on are omitted. In other words, the described transformation of permutation <span class="tex-span"><i>p</i></span> cyclically shifts to the left each consecutive block of length <span class="tex-span"><i>k</i></span> and the last block with the length equal to the remainder after dividing <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>k</i></span>. </p><p>John Doe thinks that permutation <span class="tex-span"><i>f</i>(<i>f</i>(&nbsp;...&nbsp;<i>f</i>(<i>p</i> = [1, 2, ..., <i>n</i>], 2)&nbsp;...&nbsp;, <i>n</i> - 1), <i>n</i>)</span> is beautiful. Unfortunately, he cannot quickly find the beautiful permutation he's interested in. That's why he asked you to help him.</p><p>Your task is to find a beautiful permutation for the given <span class="tex-span"><i>n</i></span>. For clarifications, see the notes to the third sample.</p></div><div class="input-specification"><p>A single line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> distinct space-separated integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — a beautiful permutation of size <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>A single line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> distinct space-separated integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — a beautiful permutation of size <span class="tex-span"><i>n</i></span>.</p>





```input1
2

```




```input2
3

```




```input3
4

```




```output1
2 1 

```




```output2
1 3 2 

```




```output3
4 2 3 1 

```



## Note

<p>A note to the third test sample: </p><ul> <li> <span class="tex-span"><i>f</i>([1, 2, 3, 4], 2) = [2, 1, 4, 3]</span> </li><li> <span class="tex-span"><i>f</i>([2, 1, 4, 3], 3) = [1, 4, 2, 3]</span> </li><li> <span class="tex-span"><i>f</i>([1, 4, 2, 3], 4) = [4, 2, 3, 1]</span> </li></ul>
