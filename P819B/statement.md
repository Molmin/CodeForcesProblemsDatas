## Description

<div><p>Some time ago Mister B detected a strange signal from the space, which he started to study.</p><p>After some transformation the signal turned out to be a permutation <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span> or its cyclic shift. For the further investigation Mister B need some basis, that's why he decided to choose cyclic shift of this permutation which has the minimum possible deviation.</p><p>Let's define the deviation of a permutation <span class="tex-span"><i>p</i></span> as <img align="middle" class="tex-formula" src="file://BMYgm0iL.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Find a cyclic shift of permutation <span class="tex-span"><i>p</i></span> with minimum possible deviation. If there are multiple solutions, print any of them.</p><p>Let's denote id <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> &lt; <i>n</i></span>) of a cyclic shift of permutation <span class="tex-span"><i>p</i></span> as the number of right shifts needed to reach this shift, for example:</p><ul> <li> <span class="tex-span"><i>k</i> = 0</span>: shift <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub></span>, </li><li> <span class="tex-span"><i>k</i> = 1</span>: shift <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i></sub>, <i>p</i><sub class="lower-index">1</sub>, ... <i>p</i><sub class="lower-index"><i>n</i> - 1</sub></span>, </li><li> ..., </li><li> <span class="tex-span"><i>k</i> = <i>n</i> - 1</span>: shift <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ... <i>p</i><sub class="lower-index"><i>n</i></sub>, <i>p</i><sub class="lower-index">1</sub></span>. </li></ul></div><div class="input-specification"><p>First line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the elements of the permutation. It is guaranteed that all elements are distinct.</p></div><div class="output-specification"><p>Print two integers: the minimum deviation of cyclic shifts of permutation <span class="tex-span"><i>p</i></span> and the id of such shift. If there are multiple solutions, print any of them.</p></div>

## Input

<p>First line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the length of the permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the elements of the permutation. It is guaranteed that all elements are distinct.</p>

## Output

<p>Print two integers: the minimum deviation of cyclic shifts of permutation <span class="tex-span"><i>p</i></span> and the id of such shift. If there are multiple solutions, print any of them.</p>





```input1
3
1 2 3

```




```input2
3
2 3 1

```




```input3
3
3 2 1

```




```output1
0 0

```




```output2
0 1

```




```output3
2 1

```



## Note

<p>In the first sample test the given permutation <span class="tex-span"><i>p</i></span> is the identity permutation, that's why its deviation equals to <span class="tex-span">0</span>, the shift id equals to <span class="tex-span">0</span> as well.</p><p>In the second sample test the deviation of <span class="tex-span"><i>p</i></span> equals to <span class="tex-span">4</span>, the deviation of the <span class="tex-span">1</span>-st cyclic shift <span class="tex-span">(1, 2, 3)</span> equals to <span class="tex-span">0</span>, the deviation of the <span class="tex-span">2</span>-nd cyclic shift <span class="tex-span">(3, 1, 2)</span> equals to <span class="tex-span">4</span>, the optimal is the <span class="tex-span">1</span>-st cyclic shift.</p><p>In the third sample test the deviation of <span class="tex-span"><i>p</i></span> equals to <span class="tex-span">4</span>, the deviation of the <span class="tex-span">1</span>-st cyclic shift <span class="tex-span">(1, 3, 2)</span> equals to <span class="tex-span">2</span>, the deviation of the <span class="tex-span">2</span>-nd cyclic shift <span class="tex-span">(2, 1, 3)</span> also equals to <span class="tex-span">2</span>, so the optimal are both <span class="tex-span">1</span>-st and <span class="tex-span">2</span>-nd cyclic shifts.</p>
