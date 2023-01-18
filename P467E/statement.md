## Description

<div><p>After you have read all the problems, probably, you think Alex is genius person. That's true! One day he came up with the following task.</p><p>Given a sequence of integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. You are to find a longest sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index">4<i>m</i></sub></span>, that satisfies the following conditions:</p><ul> <li> <span class="tex-span"><i>b</i><sub class="lower-index">4<i>k</i> + 1</sub> = <i>b</i><sub class="lower-index">4<i>k</i> + 3</sub></span> for all valid integer <span class="tex-span"><i>k</i></span>; </li><li> <span class="tex-span"><i>b</i><sub class="lower-index">4<i>k</i> + 2</sub> = <i>b</i><sub class="lower-index">4<i>k</i> + 4</sub></span> for all valid integer <span class="tex-span"><i>k</i></span>; </li><li> sequence <span class="tex-span"><i>b</i></span> is subsequence of <span class="tex-span"><i>a</i></span> (not necessarily contiguous subsequence). </li></ul><p>And finally... Alex had given this complicated task to George, and George gave it to you. Help George to cope with the task.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span">4<i>m</i></span> — the maximal possible length of required sequence <span class="tex-span"><i>b</i></span>. In the second line print <span class="tex-span">4<i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index">4<i>m</i></sub></span>, that is required sequence.</p><p>If there are multiple optimal answers you may print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>In the first line print a single integer <span class="tex-span">4<i>m</i></span> — the maximal possible length of required sequence <span class="tex-span"><i>b</i></span>. In the second line print <span class="tex-span">4<i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index">4<i>m</i></sub></span>, that is required sequence.</p><p>If there are multiple optimal answers you may print any of them.</p>





```input1
4
3 5 3 5

```




```input2
10
35 1 2 1 2 35 100 200 100 200

```




```output1
4
3 5 3 5

```




```output2
8
1 2 1 2 100 200 100 200

```


