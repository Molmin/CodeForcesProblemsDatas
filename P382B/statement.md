## Description

<div><p>Arthur and Alexander are number busters. Today they've got a competition. </p><p>Arthur took a group of four integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>w</i>, <i>x</i></span> <span class="tex-span">(0 ≤ <i>b</i> &lt; <i>w</i>, 0 &lt; <i>x</i> &lt; <i>w</i>)</span> and Alexander took integer <span class="tex-span"><i>с</i></span>. Arthur and Alexander use distinct approaches to number bustings. Alexander is just a regular guy. Each second, he subtracts one from his number. In other words, he performs the assignment: <span class="tex-span"><i>c</i> = <i>c</i> - 1</span>. Arthur is a sophisticated guy. Each second Arthur performs a complex operation, described as follows: if <span class="tex-span"><i>b</i> ≥ <i>x</i></span>, perform the assignment <span class="tex-span"><i>b</i> = <i>b</i> - <i>x</i></span>, if <span class="tex-span"><i>b</i> &lt; <i>x</i></span>, then perform two consecutive assignments <span class="tex-span"><i>a</i> = <i>a</i> - 1;&nbsp;<i>b</i> = <i>w</i> - (<i>x</i> - <i>b</i>)</span>.</p><p>You've got numbers <span class="tex-span"><i>a</i>, <i>b</i>, <i>w</i>, <i>x</i>, <i>c</i></span>. Determine when Alexander gets ahead of Arthur if both guys start performing the operations at the same time. Assume that Alexander got ahead of Arthur if <span class="tex-span"><i>c</i> ≤ <i>a</i></span>.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>w</i>, <i>x</i>, <i>c</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 2·10<sup class="upper-index">9</sup>, 1 ≤ <i>w</i> ≤ 1000, 0 ≤ <i>b</i> &lt; <i>w</i>, 0 &lt; <i>x</i> &lt; <i>w</i>, 1 ≤ <i>c</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum time in seconds Alexander needs to get ahead of Arthur. You can prove that the described situation always occurs within the problem's limits.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>a</i>, <i>b</i>, <i>w</i>, <i>x</i>, <i>c</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ 2·10<sup class="upper-index">9</sup>, 1 ≤ <i>w</i> ≤ 1000, 0 ≤ <i>b</i> &lt; <i>w</i>, 0 &lt; <i>x</i> &lt; <i>w</i>, 1 ≤ <i>c</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print a single integer — the minimum time in seconds Alexander needs to get ahead of Arthur. You can prove that the described situation always occurs within the problem's limits.</p>





```input1
4 2 3 1 6

```




```input2
4 2 3 1 7

```




```input3
1 2 3 2 6

```




```input4
1 1 2 1 1

```




```output1
2

```




```output2
4

```




```output3
13

```




```output4
0

```


