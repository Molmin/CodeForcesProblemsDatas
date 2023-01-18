## Description

<div><p>Mike has discovered a new way to encode permutations. If he has a permutation <span class="tex-span"><i>P</i> = [<i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub>]</span>, he will encode it in the following way:</p><p>Denote by <span class="tex-span"><i>A</i> = [<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>]</span> a sequence of length <span class="tex-span"><i>n</i></span> which will represent the code of the permutation. For each <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> sequentially, he will choose the smallest unmarked <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) such that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i><sub class="lower-index"><i>j</i></sub></span> and will assign to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> the number <span class="tex-span"><i>j</i></span> (in other words he performs <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>j</i></span>) and will mark <span class="tex-span"><i>j</i></span>. If there is no such <span class="tex-span"><i>j</i></span>, he'll assign to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> the number <span class="tex-span"> - 1</span> (he performs <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> =  - 1</span>). </p><p>Mike forgot his original permutation but he remembers its code. Your task is simple: find <span class="tex-font-style-bf">any</span> permutation such that its code is the same as the code of Mike's original permutation.</p><p>You may assume that there will always be at least one valid permutation.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>) — length of permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> =  - 1</span>) — the code of Mike's permutation.</p><p>You may assume that all positive values from <span class="tex-span"><i>A</i></span> are different.</p></div><div class="output-specification"><p>In first and only line print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — a permutation <span class="tex-span"><i>P</i></span> which has the same code as the given one. Note that numbers in permutation are distinct.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>) — length of permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> =  - 1</span>) — the code of Mike's permutation.</p><p>You may assume that all positive values from <span class="tex-span"><i>A</i></span> are different.</p>

## Output

<p>In first and only line print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — a permutation <span class="tex-span"><i>P</i></span> which has the same code as the given one. Note that numbers in permutation are distinct.</p>





```input1
6
2 -1 1 5 -1 4

```




```input2
8
2 -1 4 -1 6 -1 8 -1

```




```output1
2 6 1 4 5 3

```




```output2
1 8 2 7 3 6 4 5

```



## Note

<p>For the permutation from the first example:</p><p><span class="tex-span"><i>i</i> = 1</span>, the smallest <span class="tex-span"><i>j</i></span> is <span class="tex-span">2</span> because <span class="tex-span"><i>p</i><sub class="lower-index">2</sub> = 6 &gt; <i>p</i><sub class="lower-index">1</sub> = 2</span>.</p><p><span class="tex-span"><i>i</i> = 2</span>, there is no <span class="tex-span"><i>j</i></span> because <span class="tex-span"><i>p</i><sub class="lower-index">2</sub> = 6</span> is the greatest element in the permutation.</p><p><span class="tex-span"><i>i</i> = 3</span>, the smallest <span class="tex-span"><i>j</i></span> is <span class="tex-span">1</span> because <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = 2 &gt; <i>p</i><sub class="lower-index">3</sub> = 1</span>.</p><p><span class="tex-span"><i>i</i> = 4</span>, the smallest <span class="tex-span"><i>j</i></span> is <span class="tex-span">5</span> (<span class="tex-span">2</span> was already marked) because <span class="tex-span"><i>p</i><sub class="lower-index">5</sub> = 5 &gt; <i>p</i><sub class="lower-index">4</sub> = 4</span>.</p><p><span class="tex-span"><i>i</i> = 5</span>, there is no <span class="tex-span"><i>j</i></span> because <span class="tex-span">2</span> is already marked.</p><p><span class="tex-span"><i>i</i> = 6</span>, the smallest <span class="tex-span"><i>j</i></span> is <span class="tex-span">4</span> because <span class="tex-span"><i>p</i><sub class="lower-index">4</sub> = 4 &gt; <i>p</i><sub class="lower-index">6</sub> = 3</span>.</p>
