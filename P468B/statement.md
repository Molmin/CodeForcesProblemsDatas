## Description

<div><p>Little X has <span class="tex-span"><i>n</i></span> distinct integers: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span>. He wants to divide all of them into two sets <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>. The following two conditions must be satisfied:</p><ul> <li> If number <span class="tex-span"><i>x</i></span> belongs to set <span class="tex-span"><i>A</i></span>, then number <span class="tex-span"><i>a</i> - <i>x</i></span> must also belong to set <span class="tex-span"><i>A</i></span>. </li><li> If number <span class="tex-span"><i>x</i></span> belongs to set <span class="tex-span"><i>B</i></span>, then number <span class="tex-span"><i>b</i> - <i>x</i></span> must also belong to set <span class="tex-span"><i>B</i></span>. </li></ul><p>Help Little X divide the numbers into two sets or determine that it's impossible.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>If there is a way to divide the numbers into two sets, then print "<span class="tex-font-style-tt">YES</span>" in the first line. Then print <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals either <span class="tex-span">0</span>, or <span class="tex-span">1</span>), describing the division. If <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals to <span class="tex-span">0</span>, then <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> belongs to set <span class="tex-span"><i>A</i></span>, otherwise it belongs to set <span class="tex-span"><i>B</i></span>.</p><p>If it's impossible, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>a</i>, <i>b</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> space-separated distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>If there is a way to divide the numbers into two sets, then print "<span class="tex-font-style-tt">YES</span>" in the first line. Then print <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals either <span class="tex-span">0</span>, or <span class="tex-span">1</span>), describing the division. If <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals to <span class="tex-span">0</span>, then <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> belongs to set <span class="tex-span"><i>A</i></span>, otherwise it belongs to set <span class="tex-span"><i>B</i></span>.</p><p>If it's impossible, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
4 5 9
2 3 4 5

```




```input2
3 3 4
1 2 4

```




```output1
YES
0 0 1 1

```




```output2
NO

```



## Note

<p>It's OK if all the numbers are in the same set, and the other one is empty.</p>
