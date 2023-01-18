## Description

<div><p>Sereja is interested in intervals of numbers, so he has prepared a problem about intervals for you. An interval of numbers is a pair of integers <span class="tex-span">[<i>l</i>, <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>m</i>)</span>. Interval <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span> belongs to interval <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>]</span> if the following condition is met: <span class="tex-span"><i>l</i><sub class="lower-index">2</sub> ≤ <i>l</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">2</sub></span>.</p><p>Sereja wants to write out a sequence of <span class="tex-span"><i>n</i></span> intervals <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span>, <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>]</span>, <span class="tex-span">...</span>, <span class="tex-span">[<i>l</i><sub class="lower-index"><i>n</i></sub>, <i>r</i><sub class="lower-index"><i>n</i></sub>]</span> on a piece of paper. At that, no interval in the sequence can belong to some other interval of the sequence. Also, Sereja loves number <span class="tex-span"><i>x</i></span> very much and he wants some (at least one) interval in the sequence to have <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>x</i></span>. Sereja wonders, how many distinct ways to write such intervals are there?</p><p>Help Sereja and find the required number of ways modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>Two ways are considered distinct if there is such <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>j</i> ≤ <i>n</i>)</span>, that the <span class="tex-span"><i>j</i></span>-th intervals in two corresponding sequences are not equal.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>n</i>·<i>m</i> ≤ 100000, 1 ≤ <i>x</i> ≤ <i>m</i>)</span> — the number of segments in the sequence, the constraints on the numbers in segments and Sereja's favourite number.</p></div><div class="output-specification"><p>In a single line print the answer modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>n</i>·<i>m</i> ≤ 100000, 1 ≤ <i>x</i> ≤ <i>m</i>)</span> — the number of segments in the sequence, the constraints on the numbers in segments and Sereja's favourite number.</p>

## Output

<p>In a single line print the answer modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1 1 1

```




```input2
3 5 1

```




```input3
2 3 3

```




```output1
1

```




```output2
240

```




```output3
6

```



## Note

<p>In third example next sequences will be correct: <span class="tex-span">{[1, 1], [3, 3]}</span>, <span class="tex-span">{[1, 2], [3, 3]}</span>, <span class="tex-span">{[2, 2], [3, 3]}</span>, <span class="tex-span">{[3, 3], [1, 1]}</span>, <span class="tex-span">{[3, 3], [2, 2]}</span>, <span class="tex-span">{[3, 3], [1, 2]}</span>.</p>
