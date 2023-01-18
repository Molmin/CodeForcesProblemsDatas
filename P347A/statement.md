## Description

<div><p>You want to arrange <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> in some order in a row. Let's define the value of an arrangement as the sum of differences between all pairs of adjacent integers.</p><p>More formally, let's denote some arrangement as a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, where sequence <span class="tex-span"><i>x</i></span> is a permutation of sequence <span class="tex-span"><i>a</i></span>. The value of such an arrangement is <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub> - <i>x</i><sub class="lower-index">2</sub>) + (<i>x</i><sub class="lower-index">2</sub> - <i>x</i><sub class="lower-index">3</sub>) + ... + (<i>x</i><sub class="lower-index"><i>n</i> - 1</sub> - <i>x</i><sub class="lower-index"><i>n</i></sub>)</span>.</p><p>Find the largest possible value of an arrangement. Then, output the lexicographically smallest sequence <span class="tex-span"><i>x</i></span> that corresponds to an arrangement of the largest possible value.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000</span>).</p></div><div class="output-specification"><p>Print the required sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. Sequence <span class="tex-span"><i>x</i></span> should be the lexicographically smallest permutation of <span class="tex-span"><i>a</i></span> that corresponds to an arrangement of the largest possible value.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 1000</span>).</p>

## Output

<p>Print the required sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. Sequence <span class="tex-span"><i>x</i></span> should be the lexicographically smallest permutation of <span class="tex-span"><i>a</i></span> that corresponds to an arrangement of the largest possible value.</p>





```input1
5
100 -100 50 0 -50

```




```output1
100 -50 0 50 -100 

```



## Note

<p>In the sample test case, the value of the output arrangement is <span class="tex-span">(100 - ( - 50)) + (( - 50) - 0) + (0 - 50) + (50 - ( - 100)) = 200</span>. No other arrangement has a larger value, and among all arrangements with the value of <span class="tex-span">200</span>, the output arrangement is the lexicographically smallest one.</p><p>Sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>p</i></sub></span> is <span class="tex-font-style-it">lexicographically smaller</span> than sequence <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ... , <i>y</i><sub class="lower-index"><i>p</i></sub></span> if there exists an integer <span class="tex-span"><i>r</i></span> <span class="tex-span">(0 ≤ <i>r</i> &lt; <i>p</i>)</span> such that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ... , <i>x</i><sub class="lower-index"><i>r</i></sub> = <i>y</i><sub class="lower-index"><i>r</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>r</i> + 1</sub> &lt; <i>y</i><sub class="lower-index"><i>r</i> + 1</sub></span>.</p>
