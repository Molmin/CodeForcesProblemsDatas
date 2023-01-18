## Description

<div><p>Sereja has two sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> and number <span class="tex-span"><i>p</i></span>. Sequence <span class="tex-span"><i>a</i></span> consists of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Similarly, sequence <span class="tex-span"><i>b</i></span> consists of <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span>. As usual, Sereja studies the sequences he has. Today he wants to find the number of positions <span class="tex-span"><i>q</i></span> <span class="tex-span">(<i>q</i> + (<i>m</i> - 1)·<i>p</i> ≤ <i>n</i>;&nbsp;<i>q</i> ≥ 1)</span>, such that sequence <span class="tex-span"><i>b</i></span> can be obtained from sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>q</i></sub>, <i>a</i><sub class="lower-index"><i>q</i> + <i>p</i></sub>, <i>a</i><sub class="lower-index"><i>q</i> + 2<i>p</i></sub>, ..., <i>a</i><sub class="lower-index"><i>q</i> + (<i>m</i> - 1)<i>p</i></sub></span> by rearranging elements.</p><p>Sereja needs to rush to the gym, so he asked to find all the described positions of <span class="tex-span"><i>q</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>p</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>In the first line print the number of valid <span class="tex-span"><i>q</i></span>s. In the second line, print the valid values in the increasing order.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>, 1 ≤ <i>p</i> ≤ 2·10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>In the first line print the number of valid <span class="tex-span"><i>q</i></span>s. In the second line, print the valid values in the increasing order.</p>





```input1
5 3 1
1 2 3 2 1
1 2 3

```




```input2
6 3 2
1 3 2 2 3 1
1 2 3

```




```output1
2
1 3

```




```output2
2
1 2

```


