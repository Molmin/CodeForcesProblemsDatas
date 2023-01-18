## Description

<div><p>A student of <span class="tex-span"><i>z</i></span>-school found a kind of sorting called <span class="tex-span"><i>z</i></span>-sort. The array <span class="tex-span"><i>a</i></span> with <span class="tex-span"><i>n</i></span> elements are <span class="tex-span"><i>z</i></span>-sorted if two conditions hold:</p><ol> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span> for all even <span class="tex-span"><i>i</i></span>, </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span> for all odd <span class="tex-span"><i>i</i> &gt; 1</span>. </li></ol><p>For example the arrays <span class="tex-font-style-tt">[1,2,1,2]</span> and <span class="tex-font-style-tt">[1,1,1,1]</span> are <span class="tex-span"><i>z</i></span>-sorted while the array <span class="tex-font-style-tt">[1,2,3,4]</span> isn’t <span class="tex-span"><i>z</i></span>-sorted.</p><p>Can you make the array <span class="tex-span"><i>z</i></span>-sorted?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of elements in the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>If it's possible to make the array <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>z</i></span>-sorted print <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the elements after <span class="tex-span"><i>z</i></span>-sort. Otherwise print the only word "<span class="tex-font-style-tt">Impossible</span>".</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of elements in the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the elements of the array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>If it's possible to make the array <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>z</i></span>-sorted print <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the elements after <span class="tex-span"><i>z</i></span>-sort. Otherwise print the only word "<span class="tex-font-style-tt">Impossible</span>".</p>





```input1
4
1 2 2 1

```




```input2
5
1 3 2 2 5

```




```output1
1 2 1 2

```




```output2
1 5 2 3 2

```


