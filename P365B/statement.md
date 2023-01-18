## Description

<div><p>You have array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) is good if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i> - 1</sub> + <i>a</i><sub class="lower-index"><i>i</i> - 2</sub></span>, for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(<i>l</i> + 2 ≤ <i>i</i> ≤ <i>r</i>)</span>.</p><p>Let's define <span class="tex-span"><i>len</i>([<i>l</i>, <i>r</i>]) = <i>r</i> - <i>l</i> + 1</span>, <span class="tex-span"><i>len</i>([<i>l</i>, <i>r</i>])</span> is the length of the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>. Segment <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span>, is longer than segment <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>]</span>, if <span class="tex-span"><i>len</i>([<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]) &gt; <i>len</i>([<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>])</span>.</p><p>Your task is to find a good segment of the maximum length in array <span class="tex-span"><i>a</i></span>. Note that a segment of length <span class="tex-span">1</span> or <span class="tex-span">2</span> is always good.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the array. The second line contains integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the length of the longest good segment in array <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the array. The second line contains integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the length of the longest good segment in array <span class="tex-span"><i>a</i></span>.</p>





```input1
10
1 2 3 5 8 13 21 34 55 89

```




```input2
5
1 1 1 1 1

```




```output1
10

```




```output2
2

```


