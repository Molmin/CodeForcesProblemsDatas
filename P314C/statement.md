## Description

<div><p>Sereja has a sequence that consists of <span class="tex-span"><i>n</i></span> positive integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>First Sereja took a piece of squared paper and wrote all <span class="tex-font-style-bf">distinct</span> non-empty non-decreasing subsequences of sequence <span class="tex-span"><i>a</i></span>. Then for each sequence written on the squared paper, Sereja wrote on a piece of lines paper all sequences that <span class="tex-font-style-it">do not exceed</span> it.</p><p>A sequence of positive integers <span class="tex-span"><i>x</i> = <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>r</i></sub></span> doesn't exceed a sequence of positive integers <span class="tex-span"><i>y</i> = <i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>r</i></sub></span>, if the following inequation holds: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>r</i></sub> ≤ <i>y</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>Now Sereja wonders, how many sequences are written on the lines piece of paper. Help Sereja, find the required quantity modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. </p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>In the single line print the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>In the single line print the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1
42

```




```input2
3
1 2 2

```




```input3
5
1 2 3 4 5

```




```output1
42

```




```output2
13

```




```output3
719

```


