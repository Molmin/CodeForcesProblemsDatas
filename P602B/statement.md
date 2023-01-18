## Description

<div><p>When Xellos was doing a practice course in university, he once had to measure the intensity of an effect that slowly approached equilibrium. A good way to determine the equilibrium intensity would be choosing a sufficiently large number of consecutive data points that seems as constant as possible and taking their average. Of course, with the usual sizes of data, it's nothing challenging&nbsp;— but why not make a similar programming contest problem while we're at it?</p><p>You're given a sequence of <span class="tex-span"><i>n</i></span> data points <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. There aren't any big jumps between consecutive data points&nbsp;— for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>, it's guaranteed that <span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 1</span>.</p><p>A range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> of data points is said to be <span class="tex-font-style-it">almost constant</span> if the difference between the largest and the smallest value in that range is at most <span class="tex-span">1</span>. Formally, let <span class="tex-span"><i>M</i></span> be the maximum and <span class="tex-span"><i>m</i></span> the minimum value of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span>; the range <span class="tex-span">[<i>l</i>, <i>r</i>]</span> is almost constant if <span class="tex-span"><i>M</i> - <i>m</i> ≤ 1</span>.</p><p>Find the length of the longest almost constant range.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of data points.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>).</p></div><div class="output-specification"><p>Print a single number&nbsp;— the maximum length of an almost constant range of the given sequence.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of data points.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>).</p>

## Output

<p>Print a single number&nbsp;— the maximum length of an almost constant range of the given sequence.</p>





```input1
5
1 2 3 3 2

```




```input2
11
5 4 5 5 6 7 8 8 8 7 6

```




```output1
4

```




```output2
5

```



## Note

<p>In the first sample, the longest almost constant range is <span class="tex-span">[2, 5]</span>; its length (the number of data points in it) is 4.</p><p>In the second sample, there are three almost constant ranges of length <span class="tex-span">4</span>: <span class="tex-span">[1, 4]</span>, <span class="tex-span">[6, 9]</span> and <span class="tex-span">[7, 10]</span>; the only almost constant range of the maximum length <span class="tex-span">5</span> is <span class="tex-span">[6, 10]</span>.</p>
