## Description

<div><p>You are given a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of one-dimensional segments numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Your task is to find two distinct indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that segment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> lies within segment <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Segment <span class="tex-span">[<i>l</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">1</sub>]</span> lies within segment <span class="tex-span">[<i>l</i><sub class="lower-index">2</sub>, <i>r</i><sub class="lower-index">2</sub>]</span> iff <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> ≥ <i>l</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">1</sub> ≤ <i>r</i><sub class="lower-index">2</sub></span>.</p><p>Print indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. If there are multiple answers, print any of them. If no answer exists, print <span class="tex-font-style-tt">-1 -1</span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of segments.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the <span class="tex-span"><i>i</i></span>-th segment.</p></div><div class="output-specification"><p>Print two distinct indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that segment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> lies within segment <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>. If there are multiple answers, print any of them. If no answer exists, print <span class="tex-font-style-tt">-1 -1</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of segments.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the <span class="tex-span"><i>i</i></span>-th segment.</p>

## Output

<p>Print two distinct indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that segment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> lies within segment <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>. If there are multiple answers, print any of them. If no answer exists, print <span class="tex-font-style-tt">-1 -1</span>.</p>





```input1
5
1 10
2 9
3 9
2 3
2 9

```




```input2
3
1 5
2 6
6 20

```




```output1
2 1

```




```output2
-1 -1

```



## Note

<p>In the first example the following pairs are considered correct:</p><ul> <li> <span class="tex-span">(2, 1), (3, 1), (4, 1), (5, 1)</span> — not even touching borders; </li><li> <span class="tex-span">(3, 2), (4, 2), (3, 5), (4, 5)</span> — touch one border; </li><li> <span class="tex-span">(5, 2), (2, 5)</span> — match exactly. </li></ul>
