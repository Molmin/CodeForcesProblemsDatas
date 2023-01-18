## Description

<div><p>Peter has a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Peter wants all numbers in the sequence to equal <span class="tex-span"><i>h</i></span>. He can perform the operation of "adding one on the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>": add one to all elements of the sequence with indices from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (inclusive). At that, Peter never chooses any element as the beginning of the segment twice. Similarly, Peter never chooses any element as the end of the segment twice. In other words, for any two segments <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span> and <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>]</span>, where Peter added one, the following inequalities hold: <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> ≠ <i>l</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">1</sub> ≠ <i>r</i><sub class="lower-index">2</sub></span>.</p><p>How many distinct ways are there to make all numbers in the sequence equal <span class="tex-span"><i>h</i></span>? Print this number of ways modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>. Two ways are considered distinct if one of them has a segment that isn't in the other way.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>h</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>h</i> ≤ 2000)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2000)</span>.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>h</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>h</i> ≤ 2000)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2000)</span>.</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
3 2
1 1 1

```




```input2
5 1
1 1 1 1 1

```




```input3
4 3
3 2 1 1

```




```output1
4

```




```output2
1

```




```output3
0

```


