## Description

<div><p>You are given a set <span class="tex-span"><i>Y</i></span> of <span class="tex-span"><i>n</i></span> <span class="tex-font-style-bf">distinct</span> positive integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Set <span class="tex-span"><i>X</i></span> of <span class="tex-span"><i>n</i></span> <span class="tex-font-style-bf">distinct</span> positive integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> is said to <span class="tex-font-style-it">generate</span> set <span class="tex-span"><i>Y</i></span> if one can transform <span class="tex-span"><i>X</i></span> to <span class="tex-span"><i>Y</i></span> by applying some number of the following two operation to integers in <span class="tex-span"><i>X</i></span>:</p><ol> <li> Take any integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and multiply it by two, i.e. replace <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> with <span class="tex-span">2·<i>x</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> Take any integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, multiply it by two and add one, i.e. replace <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> with <span class="tex-span">2·<i>x</i><sub class="lower-index"><i>i</i></sub> + 1</span>. </li></ol><p>Note that integers in <span class="tex-span"><i>X</i></span> are not required to be distinct after each operation.</p><p>Two sets of distinct integers <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> are equal if they are equal as sets. In other words, if we write elements of the sets in the array in the increasing order, these arrays would be equal.</p><p>Note, that any set of integers (or its permutation) generates itself.</p><p>You are given a set <span class="tex-span"><i>Y</i></span> and have to find a set <span class="tex-span"><i>X</i></span> that generates <span class="tex-span"><i>Y</i></span> and the <span class="tex-font-style-bf">maximum element of <span class="tex-span"><i>X</i></span> is mininum possible</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50 000</span>)&nbsp;— the number of elements in <span class="tex-span"><i>Y</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), that are guaranteed to be distinct.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— set of distinct integers that generate <span class="tex-span"><i>Y</i></span> and the maximum element of which is minimum possible. If there are several such sets, print any of them.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50 000</span>)&nbsp;— the number of elements in <span class="tex-span"><i>Y</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, ..., <i>y</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), that are guaranteed to be distinct.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— set of distinct integers that generate <span class="tex-span"><i>Y</i></span> and the maximum element of which is minimum possible. If there are several such sets, print any of them.</p>





```input1
5
1 2 3 4 5

```




```input2
6
15 14 3 13 1 12

```




```input3
6
9 7 13 17 5 11

```




```output1
4 5 2 3 1 

```




```output2
12 13 14 7 3 1 

```




```output3
4 5 2 6 3 1 

```


