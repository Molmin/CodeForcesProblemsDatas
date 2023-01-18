## Description

<div><p>You've got an array <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Your task is to find a minimal by inclusion segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span> such, that among numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, &nbsp;<i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, &nbsp;..., &nbsp;<i>a</i><sub class="lower-index"><i>r</i></sub></span> there are exactly <span class="tex-span"><i>k</i></span> distinct numbers.</p><p>Segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;</span> <span class="tex-span"><i>l</i>, <i>r</i></span> are integers) of length <span class="tex-span"><i>m</i> = <i>r</i> - <i>l</i> + 1</span>, satisfying the given property, is called <span class="tex-font-style-it">minimal by inclusion</span>, if there is no segment <span class="tex-span">[<i>x</i>, <i>y</i>]</span> satisfying the property and less then <span class="tex-span"><i>m</i></span> in length, such that <span class="tex-span">1 ≤ <i>l</i> ≤ <i>x</i> ≤ <i>y</i> ≤ <i>r</i> ≤ <i>n</i></span>. Note that the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> doesn't have to be minimal in length among all segments, satisfying the given property.</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— elements of the array <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print a space-separated pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) such, that the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> is the answer to the problem. If the sought segment does not exist, print "<span class="tex-font-style-tt">-1 -1</span>" without the quotes. If there are multiple correct answers, print any of them.</p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— elements of the array <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print a space-separated pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) such, that the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> is the answer to the problem. If the sought segment does not exist, print "<span class="tex-font-style-tt">-1 -1</span>" without the quotes. If there are multiple correct answers, print any of them.</p>





```input1
4 2
1 2 2 3

```




```input2
8 3
1 1 2 2 3 3 4 5

```




```input3
7 4
4 7 7 4 7 4 7

```




```output1
1 2

```




```output2
2 5

```




```output3
-1 -1

```



## Note

<p>In the first sample among numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> there are exactly two distinct numbers.</p><p>In the second sample segment <span class="tex-span">[2, 5]</span> is a minimal by inclusion segment with three distinct numbers, but it is not minimal in length among such segments.</p><p>In the third sample there is no segment with four distinct numbers.</p>
