## Description

<div><p><span class="tex-font-style-it">A dragon symbolizes wisdom, power and wealth. On Lunar New Year's Day, people model a dragon with bamboo strips and clothes, raise them with rods, and hold the rods high and low to resemble a flying dragon.</span></p><p>A performer holding the rod low is represented by a <span class="tex-span">1</span>, while one holding it high is represented by a <span class="tex-span">2</span>. Thus, the line of performers can be represented by a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Little Tommy is among them. He would like to choose an interval <span class="tex-span">[<i>l</i>, <i>r</i>]</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), then reverse <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> so that the length of the longest non-decreasing subsequence of the new sequence is maximum.</p><p>A non-decreasing subsequence is a sequence of indices <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span>, such that <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub> ≤ <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>k</i></sub></sub></span>. The length of the subsequence is <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>, denoting the length of the original sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, describing the original sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2, <i>i</i> = 1, 2, ..., <i>n</i>)</span>.</p></div><div class="output-specification"><p>Print a single integer, which means the maximum possible length of the longest non-decreasing subsequence of the new sequence.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>, denoting the length of the original sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, describing the original sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2, <i>i</i> = 1, 2, ..., <i>n</i>)</span>.</p>

## Output

<p>Print a single integer, which means the maximum possible length of the longest non-decreasing subsequence of the new sequence.</p>





```input1
4
1 2 1 2

```




```input2
10
1 1 2 2 2 1 1 2 2 1

```




```output1
4

```




```output2
9

```



## Note

<p>In the first example, after reversing <span class="tex-span">[2, 3]</span>, the array will become <span class="tex-span">[1, 1, 2, 2]</span>, where the length of the longest non-decreasing subsequence is <span class="tex-span">4</span>.</p><p>In the second example, after reversing <span class="tex-span">[3, 7]</span>, the array will become <span class="tex-span">[1, 1, 1, 1, 2, 2, 2, 2, 2, 1]</span>, where the length of the longest non-decreasing subsequence is <span class="tex-span">9</span>.</p>
