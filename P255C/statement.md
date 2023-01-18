## Description

<div><p>Gena loves sequences of numbers. Recently, he has discovered a new type of sequences which he called an almost arithmetical progression. A sequence is an <span class="tex-font-style-it">almost arithmetical progression</span>, if its elements can be represented as:</p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>p</i></span>, where <span class="tex-span"><i>p</i></span> is some integer; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i> - 1</sub> + ( - 1)<sup class="upper-index"><i>i</i> + 1</sup>·<i>q</i></span> <span class="tex-span">(<i>i</i> &gt; 1)</span>, where <span class="tex-span"><i>q</i></span> is some integer. </li></ul><p>Right now Gena has a piece of paper with sequence <span class="tex-span"><i>b</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers. Help Gena, find there the longest subsequence of integers that is an almost arithmetical progression.</p><p>Sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>,  <i>s</i><sub class="lower-index">2</sub>,  ...,  <i>s</i><sub class="lower-index"><i>k</i></sub></span> is a subsequence of sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>,  <i>b</i><sub class="lower-index">2</sub>,  ...,  <i>b</i><sub class="lower-index"><i>n</i></sub></span>, if there is such increasing sequence of indexes <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>k</i></sub></span> <span class="tex-span">(1  ≤  <i>i</i><sub class="lower-index">1</sub>  &lt;  <i>i</i><sub class="lower-index">2</sub>  &lt; ...   &lt;  <i>i</i><sub class="lower-index"><i>k</i></sub>  ≤  <i>n</i>)</span>, that <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>j</i></sub></sub>  =  <i>s</i><sub class="lower-index"><i>j</i></sub></span>. In other words, sequence <span class="tex-span"><i>s</i></span> can be obtained from <span class="tex-span"><i>b</i></span> by crossing out some elements.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 4000)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the length of the required longest subsequence.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 4000)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>Print a single integer — the length of the required longest subsequence.</p>





```input1
2
3 5

```




```input2
4
10 20 10 30

```




```output1
2

```




```output2
3

```



## Note

<p>In the first test the sequence actually is the suitable subsequence. </p><p>In the second test the following subsequence fits: <span class="tex-span">10, 20, 10</span>.</p>
