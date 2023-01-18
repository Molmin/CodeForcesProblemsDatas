## Description

<div><p><span class="tex-font-style-it">This problem differs from one which was on the online contest.</span></p><p>The sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> is called increasing, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <span class="tex-span"><i>i</i> &lt; <i>n</i></span>.</p><p>The sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span> is called the subsequence of the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, if there exist such a set of indexes <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span> that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>j</i></sub></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub></span>. In other words, the sequence <span class="tex-span"><i>s</i></span> can be derived from the sequence <span class="tex-span"><i>a</i></span> by crossing out some elements.</p><p>You are given two sequences of integer numbers. You are to find their longest common increasing subsequence, i.e. an increasing sequence of maximum length that is the subsequence of both sequences.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the length of the first sequence. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers from the range <span class="tex-span">[0, 10<sup class="upper-index">9</sup>]</span> — elements of the first sequence. The third line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 500</span>) — the length of the second sequence. The fourth line contains <span class="tex-span"><i>m</i></span> space-separated integers from the range <span class="tex-span">[0, 10<sup class="upper-index">9</sup>]</span> — elements of the second sequence.</p></div><div class="output-specification"><p>In the first line output <span class="tex-span"><i>k</i></span> — the length of the longest common increasing subsequence. In the second line output the subsequence itself. Separate the elements with a space. If there are several solutions, output any.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>) — the length of the first sequence. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers from the range <span class="tex-span">[0, 10<sup class="upper-index">9</sup>]</span> — elements of the first sequence. The third line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 500</span>) — the length of the second sequence. The fourth line contains <span class="tex-span"><i>m</i></span> space-separated integers from the range <span class="tex-span">[0, 10<sup class="upper-index">9</sup>]</span> — elements of the second sequence.</p>

## Output

<p>In the first line output <span class="tex-span"><i>k</i></span> — the length of the longest common increasing subsequence. In the second line output the subsequence itself. Separate the elements with a space. If there are several solutions, output any.</p>





```input1
7
2 3 1 6 5 4 6
4
1 3 5 6

```




```input2
5
1 2 0 2 1
3
1 0 1

```




```output1
3
3 5 6 

```




```output2
2
0 1 

```


