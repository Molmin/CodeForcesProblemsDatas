## Description

<div><p>Little Dima has two sequences of points with integer coordinates: sequence <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, 1), (<i>a</i><sub class="lower-index">2</sub>, 2), ..., (<i>a</i><sub class="lower-index"><i>n</i></sub>, <i>n</i>)</span> and sequence <span class="tex-span">(<i>b</i><sub class="lower-index">1</sub>, 1), (<i>b</i><sub class="lower-index">2</sub>, 2), ..., (<i>b</i><sub class="lower-index"><i>n</i></sub>, <i>n</i>)</span>.</p><p>Now Dima wants to count the number of distinct sequences of points of length <span class="tex-span">2·<i>n</i></span> that can be assembled from these sequences, such that the <span class="tex-span"><i>x</i></span>-coordinates of points in the assembled sequence will <span class="tex-font-style-bf">not decrease</span>. Help him with that. Note that each element of the initial sequences should be used exactly once in the assembled sequence.</p><p>Dima considers two assembled sequences <span class="tex-span">(<i>p</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">1</sub>), (<i>p</i><sub class="lower-index">2</sub>, <i>q</i><sub class="lower-index">2</sub>), ..., (<i>p</i><sub class="lower-index">2·<i>n</i></sub>, <i>q</i><sub class="lower-index">2·<i>n</i></sub>)</span> and <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>), (<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>), ..., (<i>x</i><sub class="lower-index">2·<i>n</i></sub>, <i>y</i><sub class="lower-index">2·<i>n</i></sub>)</span> distinct, if there is such <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ 2·<i>n</i>)</span>, that <span class="tex-span">(<i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub>) ≠ (<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>As the answer can be rather large, print the remainder from dividing the answer by number <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The numbers in the lines are separated by spaces.</p><p>The last line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="output-specification"><p>In the single line print the remainder after dividing the answer to the problem by number <span class="tex-span"><i>m</i></span>. </p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The numbers in the lines are separated by spaces.</p><p>The last line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup> + 7)</span>.</p>

## Output

<p>In the single line print the remainder after dividing the answer to the problem by number <span class="tex-span"><i>m</i></span>. </p>





```input1
1
1
2
7

```




```input2
2
1 2
2 3
11

```




```output1
1

```




```output2
2

```



## Note

<p>In the first sample you can get only one sequence: <span class="tex-span">(1, 1), (2, 1)</span>. </p><p>In the second sample you can get such sequences : <span class="tex-span">(1, 1), (2, 2), (2, 1), (3, 2)</span>; <span class="tex-span">(1, 1), (2, 1), (2, 2), (3, 2)</span>. Thus, the answer is <span class="tex-span">2</span>.</p>
