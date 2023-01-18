## Description

<div><p>A <span class="tex-font-style-it">permutation</span> <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span> is a sequence of distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>. A permutation is an identity permutation, if for any <span class="tex-span"><i>i</i></span> the following equation holds <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span>. </p><p>A <span class="tex-font-style-it">swap</span> <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is the operation that swaps elements <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> in the permutation. Let's assume that <span class="tex-span"><i>f</i>(<i>p</i>)</span> is the minimum number of swaps that you need to make the permutation <span class="tex-span"><i>p</i></span> an identity permutation. </p><p>Valera wonders, how he can transform permutation <span class="tex-span"><i>p</i></span> into any permutation <span class="tex-span"><i>q</i></span>, such that <span class="tex-span"><i>f</i>(<i>q</i>) = <i>m</i></span>, using the minimum number of swaps. Help him do that.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>) — the length of permutation <span class="tex-span"><i>p</i></span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — Valera's initial permutation. The last line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; <i>n</i></span>).</p></div><div class="output-specification"><p>In the first line, print integer <span class="tex-span"><i>k</i></span> — the minimum number of swaps.</p><p>In the second line, print <span class="tex-span">2<i>k</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index">2<i>k</i></sub></span> — the description of the swap sequence. The printed numbers show that you need to consecutively make swaps <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>)</span>, ..., <span class="tex-span">(<i>x</i><sub class="lower-index">2<i>k</i> - 1</sub>, <i>x</i><sub class="lower-index">2<i>k</i></sub>)</span>. </p><p>If there are multiple sequence swaps of the minimum length, print the lexicographically minimum one.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>) — the length of permutation <span class="tex-span"><i>p</i></span>. The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — Valera's initial permutation. The last line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> &lt; <i>n</i></span>).</p>

## Output

<p>In the first line, print integer <span class="tex-span"><i>k</i></span> — the minimum number of swaps.</p><p>In the second line, print <span class="tex-span">2<i>k</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index">2<i>k</i></sub></span> — the description of the swap sequence. The printed numbers show that you need to consecutively make swaps <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>)</span>, <span class="tex-span">(<i>x</i><sub class="lower-index">3</sub>, <i>x</i><sub class="lower-index">4</sub>)</span>, ..., <span class="tex-span">(<i>x</i><sub class="lower-index">2<i>k</i> - 1</sub>, <i>x</i><sub class="lower-index">2<i>k</i></sub>)</span>. </p><p>If there are multiple sequence swaps of the minimum length, print the lexicographically minimum one.</p>





```input1
5
1 2 3 4 5
2

```




```input2
5
2 1 4 5 3
2

```




```output1
2
1 2 1 3
```




```output2
1
1 2
```



## Note

<p>Sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>s</i></sub></span> is lexicographically smaller than sequence <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>s</i></sub></span>, if there is such integer <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>r</i> ≤ <i>s</i>)</span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>r</i> - 1</sub> = <i>y</i><sub class="lower-index"><i>r</i> - 1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i></sub> &lt; <i>y</i><sub class="lower-index"><i>r</i></sub></span>. </p>
