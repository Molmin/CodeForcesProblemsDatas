## Description

<div><p>Squirrel Liss is interested in sequences. She also has preferences of integers. She thinks <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> are <span class="tex-font-style-it">good</span>.</p><p>Now she is interested in good sequences. A sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span> is called <span class="tex-font-style-it">good</span> if it satisfies the following three conditions:</p><ul> <li> The sequence is strictly increasing, i.e. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>x</i><sub class="lower-index"><i>i</i> + 1</sub></span> for each <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>k</i> - 1)</span>. </li><li> No two adjacent elements are coprime, i.e. <span class="tex-span"><i>gcd</i>(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i> + 1</sub>) &gt; 1</span> for each <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>k</i> - 1)</span> (where <span class="tex-span"><i>gcd</i>(<i>p</i>, <i>q</i>)</span> denotes the greatest common divisor of the integers <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span>). </li><li> All elements of the sequence are good integers. </li></ul><p>Find the length of the longest good sequence.</p></div><div class="input-specification"><p>The input consists of two lines. The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of good integers. The second line contains a single-space separated list of good integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> in strictly increasing order (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p></div><div class="output-specification"><p>Print a single integer — the length of the longest good sequence.</p></div>

## Input

<p>The input consists of two lines. The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of good integers. The second line contains a single-space separated list of good integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> in strictly increasing order (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span>).</p>

## Output

<p>Print a single integer — the length of the longest good sequence.</p>





```input1
5
2 3 4 6 9

```




```input2
9
1 2 3 5 6 7 8 9 10

```




```output1
4

```




```output2
4

```



## Note

<p>In the first example, the following sequences are examples of good sequences: [2; 4; 6; 9], [2; 4; 6], [3; 9], [6]. The length of the longest good sequence is 4.</p>
