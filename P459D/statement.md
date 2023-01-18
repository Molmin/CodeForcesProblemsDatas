## Description

<div><p>Parmida is a clever girl and she wants to participate in Olympiads this year. Of course she wants her partner to be clever too (although he's not)! Parmida has prepared the following test problem for Pashmak.</p><p>There is a sequence <span class="tex-span"><i>a</i></span> that consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Let's denote <span class="tex-span"><i>f</i>(<i>l</i>, <i>r</i>, <i>x</i>)</span> the number of indices <span class="tex-span"><i>k</i></span> such that: <span class="tex-span"><i>l</i> ≤ <i>k</i> ≤ <i>r</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> = <i>x</i></span>. His task is to calculate the number of pairs of indicies <span class="tex-span"><i>i</i>, <i>j</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i>)</span> such that <span class="tex-span"><i>f</i>(1, <i>i</i>, <i>a</i><sub class="lower-index"><i>i</i></sub>) &gt; <i>f</i>(<i>j</i>, <i>n</i>, <i>a</i><sub class="lower-index"><i>j</i></sub>)</span>.</p><p>Help Pashmak with the test.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print a single integer — the answer to the problem.</p>





```input1
7
1 2 1 1 2 2 1

```




```input2
3
1 1 1

```




```input3
5
1 2 3 4 5

```




```output1
8

```




```output2
1

```




```output3
0

```


