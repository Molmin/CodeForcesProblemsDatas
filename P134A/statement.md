## Description

<div><p>You are given a sequence of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Find all such indices <span class="tex-span"><i>i</i></span>, that the <span class="tex-span"><i>i</i></span>-th element equals the arithmetic mean of all <span class="tex-font-style-it">other</span> elements (that is all elements except for this one).</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains elements of the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). All the elements are positive integers.</p></div><div class="output-specification"><p>Print on the first line the number of the sought indices. Print on the second line the sought indices in the increasing order. All indices are integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>If the sought elements do not exist, then the first output line should contain number <span class="tex-span">0</span>. In this case you may either not print the second line or print an empty line.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains elements of the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). All the elements are positive integers.</p>

## Output

<p>Print on the first line the number of the sought indices. Print on the second line the sought indices in the increasing order. All indices are integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>If the sought elements do not exist, then the first output line should contain number <span class="tex-span">0</span>. In this case you may either not print the second line or print an empty line.</p>





```input1
5
1 2 3 4 5

```




```input2
4
50 50 50 50

```




```output1
1
3
```




```output2
4
1 2 3 4
```


