## Description

<div><p>You are given a permutation <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span>. Remove one element from permutation to make the number of records the maximum possible.</p><p>We remind that in a sequence of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> the element <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is a <span class="tex-font-style-it">record</span> if for every integer <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) the following holds: <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i></sub></span>. </p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of the permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation. All the integers are distinct.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the element that should be removed to make the number of records the maximum possible. If there are multiple such elements, print the smallest one.</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the length of the permutation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the permutation. All the integers are distinct.</p>

## Output

<p>Print the only integer&nbsp;— the element that should be removed to make the number of records the maximum possible. If there are multiple such elements, print the smallest one.</p>





```input1
1
1

```




```input2
5
5 1 2 3 4

```




```output1
1

```




```output2
5

```



## Note

<p>In the first example the only element can be removed.</p>
