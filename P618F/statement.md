## Description

<div><p>You are given two multisets <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>. Each multiset has exactly <span class="tex-span"><i>n</i></span> integers each between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> inclusive. Multisets may contain multiple copies of the same number.</p><p>You would like to find a nonempty subset of <span class="tex-span"><i>A</i></span> and a nonempty subset of <span class="tex-span"><i>B</i></span> such that the sum of elements in these subsets are equal. Subsets are also multisets, i.e. they can contain elements with equal values.</p><p>If no solution exists, print <span class="tex-span"> - 1</span>. Otherwise, print the indices of elements in any such subsets of <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> that have the same sum.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the size of both multisets.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, denoting the elements of <span class="tex-span"><i>A</i></span>. Each element will be between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> inclusive.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers, denoting the elements of <span class="tex-span"><i>B</i></span>. Each element will be between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> inclusive.</p></div><div class="output-specification"><p>If there is no solution, print a single integer <span class="tex-span"> - 1</span>. Otherwise, your solution should be printed on four lines.</p><p>The first line should contain a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>a</i></sub></span>, the size of the corresponding subset of <span class="tex-span"><i>A</i></span>. The second line should contain <span class="tex-span"><i>k</i><sub class="lower-index"><i>a</i></sub></span> distinct integers, the indices of the subset of <span class="tex-span"><i>A</i></span>.</p><p>The third line should contain a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>b</i></sub></span>, the size of the corresponding subset of <span class="tex-span"><i>B</i></span>. The fourth line should contain <span class="tex-span"><i>k</i><sub class="lower-index"><i>b</i></sub></span> distinct integers, the indices of the subset of <span class="tex-span"><i>B</i></span>.</p><p>Elements in both sets are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. If there are multiple possible solutions, print any of them.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the size of both multisets.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, denoting the elements of <span class="tex-span"><i>A</i></span>. Each element will be between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> inclusive.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers, denoting the elements of <span class="tex-span"><i>B</i></span>. Each element will be between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span> inclusive.</p>

## Output

<p>If there is no solution, print a single integer <span class="tex-span"> - 1</span>. Otherwise, your solution should be printed on four lines.</p><p>The first line should contain a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>a</i></sub></span>, the size of the corresponding subset of <span class="tex-span"><i>A</i></span>. The second line should contain <span class="tex-span"><i>k</i><sub class="lower-index"><i>a</i></sub></span> distinct integers, the indices of the subset of <span class="tex-span"><i>A</i></span>.</p><p>The third line should contain a single integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>b</i></sub></span>, the size of the corresponding subset of <span class="tex-span"><i>B</i></span>. The fourth line should contain <span class="tex-span"><i>k</i><sub class="lower-index"><i>b</i></sub></span> distinct integers, the indices of the subset of <span class="tex-span"><i>B</i></span>.</p><p>Elements in both sets are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. If there are multiple possible solutions, print any of them.</p>





```input1
10
10 10 10 10 10 10 10 10 10 10
10 9 8 7 6 5 4 3 2 1

```




```input2
5
4 4 3 3 3
2 2 2 2 5

```




```output1
1
2
3
5 8 10

```




```output2
2
2 3
2
3 5

```


