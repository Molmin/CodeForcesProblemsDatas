## Description

<div><p>Nick has some permutation consisting of <span class="tex-span"><i>p</i></span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. A segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> (<span class="tex-span"><i>l</i> ≤ <i>r</i></span>) is a set of elements <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> satisfying <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>.</p><p>Nick calls a pair of segments <span class="tex-span">[<i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>]</span> and <span class="tex-span">[<i>b</i><sub class="lower-index">0</sub>, <i>b</i><sub class="lower-index">1</sub>]</span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">0</sub> ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>b</i><sub class="lower-index">0</sub> ≤ <i>b</i><sub class="lower-index">1</sub> ≤ <i>n</i></span>) good if all their <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub> - <i>a</i><sub class="lower-index">0</sub> + <i>b</i><sub class="lower-index">1</sub> - <i>b</i><sub class="lower-index">0</sub> + 2)</span> elements, when sorted in ascending order, form an arithmetic progression with a difference of <span class="tex-span">1</span>. That is, when they sorted in ascending order, the elements are in the form <span class="tex-span">{<i>x</i>, <i>x</i> + 1, <i>x</i> + 2, ..., <i>x</i> + <i>m</i> - 1}</span>, for some <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>m</i></span>.</p><p>Your task is to find the number of distinct pairs of good segments in the given permutation. Two pairs of segments are considered distinct if the sets of elements contained in these pairs of segments are distinct. For example, any segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> <span class="tex-span">(<i>l</i> &lt; <i>r</i>)</span> can be represented as a pair of segments, as <span class="tex-span">[<i>l</i>, <i>i</i>]</span> and <span class="tex-span">[<i>i</i> + 1, <i>r</i>]</span> (<span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>). As all these pairs consist of the same set of elements, they are considered identical.</p><p>See the notes accompanying the sample tests for clarification.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the permutation size. The second line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print a single integer — the number of good pairs of segments of permutation <span class="tex-span"><i>p</i></span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the permutation size. The second line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print a single integer — the number of good pairs of segments of permutation <span class="tex-span"><i>p</i></span>.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier. </p>





```input1
3
1 2 3

```




```input2
5
1 4 5 3 2

```




```input3
5
5 4 3 1 2

```




```output1
3

```




```output2
10

```




```output3
10

```



## Note

<p>In the first sample the following pairs of segments are good: (<span class="tex-span">[1, 1]</span>, <span class="tex-span">[2, 2]</span>); (<span class="tex-span">[2, 2]</span>, <span class="tex-span">[3, 3]</span>); (<span class="tex-span">[1, 2]</span>, <span class="tex-span">[3, 3]</span>). Pair of segments (<span class="tex-span">[1, 1]</span>, <span class="tex-span">[2, 3]</span>) is by definition equivalent to pair (<span class="tex-span">[1, 2]</span>, <span class="tex-span">[3, 3]</span>), since both of them covers the same set of elements, namely <span class="tex-span">{1, 2, 3}</span>.</p><p>In the third sample the following pairs of segments are good: (<span class="tex-span">[4, 4]</span>, <span class="tex-span">[5, 5]</span>); (<span class="tex-span">[3, 3]</span>,<span class="tex-span">[4, 5]</span>); (<span class="tex-span">[2, 2]</span>,<span class="tex-span">[3, 5]</span>); (<span class="tex-span">[1, 1]</span>,<span class="tex-span">[2, 5]</span>); (<span class="tex-span">[3, 3]</span>,<span class="tex-span">[5, 5]</span>); (<span class="tex-span">[2, 3]</span>,<span class="tex-span">[5, 5]</span>); (<span class="tex-span">[1, 3]</span>,<span class="tex-span">[5, 5]</span>); (<span class="tex-span">[2, 2]</span>,<span class="tex-span">[3, 3]</span>); (<span class="tex-span">[1, 1]</span>,<span class="tex-span">[2, 3]</span>); (<span class="tex-span">[1, 1]</span>,<span class="tex-span">[2, 2]</span>). </p>
