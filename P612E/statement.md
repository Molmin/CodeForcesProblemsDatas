## Description

<div><p>A <span class="tex-font-style-it">permutation</span> of length <span class="tex-span"><i>n</i></span> is an array containing each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> exactly once. For example, <span class="tex-span"><i>q</i> = [4, 5, 1, 2, 3]</span> is a permutation. For the permutation <span class="tex-span"><i>q</i></span> the square of permutation is the permutation <span class="tex-span"><i>p</i></span> that <span class="tex-span"><i>p</i>[<i>i</i>] = <i>q</i>[<i>q</i>[<i>i</i>]]</span> for each <span class="tex-span"><i>i</i> = 1... <i>n</i></span>. For example, the square of <span class="tex-span"><i>q</i> = [4, 5, 1, 2, 3]</span> is <span class="tex-span"><i>p</i> = <i>q</i><sup class="upper-index">2</sup> = [2, 3, 4, 5, 1]</span>.</p><p>This problem is about the inverse operation: given the permutation <span class="tex-span"><i>p</i></span> you task is to find such permutation <span class="tex-span"><i>q</i></span> that <span class="tex-span"><i>q</i><sup class="upper-index">2</sup> = <i>p</i></span>. If there are several such <span class="tex-span"><i>q</i></span> find any of them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of elements in permutation <span class="tex-span"><i>p</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of permutation <span class="tex-span"><i>p</i></span>.</p></div><div class="output-specification"><p>If there is no permutation <span class="tex-span"><i>q</i></span> such that <span class="tex-span"><i>q</i><sup class="upper-index">2</sup> = <i>p</i></span> print the number "<span class="tex-font-style-tt">-1</span>".</p><p>If the answer exists print it. The only line should contain <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of the permutation <span class="tex-span"><i>q</i></span>. If there are several solutions print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of elements in permutation <span class="tex-span"><i>p</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of permutation <span class="tex-span"><i>p</i></span>.</p>

## Output

<p>If there is no permutation <span class="tex-span"><i>q</i></span> such that <span class="tex-span"><i>q</i><sup class="upper-index">2</sup> = <i>p</i></span> print the number "<span class="tex-font-style-tt">-1</span>".</p><p>If the answer exists print it. The only line should contain <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of the permutation <span class="tex-span"><i>q</i></span>. If there are several solutions print any of them.</p>





```input1
4
2 1 4 3

```




```input2
4
2 1 3 4

```




```input3
5
2 3 4 5 1

```




```output1
3 4 2 1

```




```output2
-1

```




```output3
4 5 1 2 3

```


