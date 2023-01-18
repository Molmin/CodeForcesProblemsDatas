## Description

<div><p>Mike is the president of country What-The-Fatherland. There are <span class="tex-span"><i>n</i></span> bears living in this country besides Mike. All of them are standing in a line and they are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. <span class="tex-span"><i>i</i></span>-th bear is exactly <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> feet high. </p><center> <img class="tex-graphics" src="file://jApqYP1p.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A group of bears is a non-empty contiguous segment of the line. The <span class="tex-font-style-it">size</span> of a group is the number of bears in that group. The <span class="tex-font-style-it">strength</span> of a group is the minimum height of the bear in that group.</p><p>Mike is a curious to know for each <span class="tex-span"><i>x</i></span> such that <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span> the maximum strength among all groups of size <span class="tex-span"><i>x</i></span>.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>), the number of bears.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers separated by space, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), heights of bears.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers in one line. For each <span class="tex-span"><i>x</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, print the maximum strength among all groups of size <span class="tex-span"><i>x</i></span>.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>), the number of bears.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers separated by space, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), heights of bears.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers in one line. For each <span class="tex-span"><i>x</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, print the maximum strength among all groups of size <span class="tex-span"><i>x</i></span>.</p>





```input1
10
1 2 3 4 5 4 3 2 1 6

```




```output1
6 4 4 3 3 2 2 1 1 1 

```


