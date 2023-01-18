## Description

<div><p>You are given a sequence of n integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>Determine a real number <span class="tex-span"><i>x</i></span> such that the <span class="tex-font-style-it">weakness</span> of the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> - <i>x</i>, <i>a</i><sub class="lower-index">2</sub> - <i>x</i>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub> - <i>x</i></span> is as small as possible.</p><p>The <span class="tex-font-style-it">weakness</span> of a sequence is defined as the maximum value of the <span class="tex-font-style-it">poorness</span> over all segments (contiguous subsequences) of a sequence.</p><p>The <span class="tex-font-style-it">poorness</span> of a segment is defined as the absolute value of sum of the elements of segment.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>), the length of a sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10 000</span>).</p></div><div class="output-specification"><p>Output a real number denoting the minimum possible <span class="tex-font-style-it">weakness</span> of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> - <i>x</i>, <i>a</i><sub class="lower-index">2</sub> - <i>x</i>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub> - <i>x</i></span>. Your answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>), the length of a sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10 000</span>).</p>

## Output

<p>Output a real number denoting the minimum possible <span class="tex-font-style-it">weakness</span> of <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> - <i>x</i>, <i>a</i><sub class="lower-index">2</sub> - <i>x</i>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub> - <i>x</i></span>. Your answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3
1 2 3

```




```input2
4
1 2 3 4

```




```input3
10
1 10 2 9 3 8 4 7 5 6

```




```output1
1.000000000000000

```




```output2
2.000000000000000

```




```output3
4.500000000000000

```



## Note

<p>For the first case, the optimal value of <span class="tex-span"><i>x</i></span> is <span class="tex-span">2</span> so the sequence becomes <span class="tex-span"> - 1</span>, <span class="tex-span">0</span>, <span class="tex-span">1</span> and the max poorness occurs at the segment "-1" or segment "1". The poorness value (answer) equals to <span class="tex-span">1</span> in this case. </p><p>For the second sample the optimal value of <span class="tex-span"><i>x</i></span> is <span class="tex-span">2.5</span> so the sequence becomes <span class="tex-span"> - 1.5,  - 0.5, 0.5, 1.5</span> and the max poorness occurs on segment "-1.5 -0.5" or "0.5 1.5". The poorness value (answer) equals to <span class="tex-span">2</span> in this case.</p>
