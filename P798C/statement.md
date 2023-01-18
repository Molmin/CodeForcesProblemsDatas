## Description

<div><p>Mike has a sequence <span class="tex-span"><i>A</i> = [<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>]</span> of length <span class="tex-span"><i>n</i></span>. He considers the sequence <span class="tex-span"><i>B</i> = [<i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub>]</span> beautiful if the <span class="tex-span"><i>gcd</i></span> of all its elements is bigger than <span class="tex-span">1</span>, i.e. <img align="middle" class="tex-formula" src="file://JWXDYqs3.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Mike wants to change his sequence in order to make it beautiful. In one move he can choose an index <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>), delete numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> and put numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, <i>a</i><sub class="lower-index"><i>i</i></sub> + <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> in their place instead, in this order. He wants perform as few operations as possible. Find the minimal number of operations to make sequence <span class="tex-span"><i>A</i></span> beautiful if it's possible, or tell him that it is impossible to do so.</p><p><img align="middle" class="tex-formula" src="file://TH5wobot.png" style="max-width: 100.0%;max-height: 100.0%;"> is the biggest non-negative number <span class="tex-span"><i>d</i></span> such that <span class="tex-span"><i>d</i></span> divides <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> for every <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) — length of sequence <span class="tex-span"><i>A</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of sequence <span class="tex-span"><i>A</i></span>.</p></div><div class="output-specification"><p>Output on the first line "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to make sequence <span class="tex-span"><i>A</i></span> beautiful by performing operations described above, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>If the answer was "<span class="tex-font-style-tt">YES</span>", output the minimal number of moves needed to make sequence <span class="tex-span"><i>A</i></span> beautiful.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) — length of sequence <span class="tex-span"><i>A</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of sequence <span class="tex-span"><i>A</i></span>.</p>

## Output

<p>Output on the first line "<span class="tex-font-style-tt">YES</span>" (without quotes) if it is possible to make sequence <span class="tex-span"><i>A</i></span> beautiful by performing operations described above, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>If the answer was "<span class="tex-font-style-tt">YES</span>", output the minimal number of moves needed to make sequence <span class="tex-span"><i>A</i></span> beautiful.</p>





```input1
2
1 1

```




```input2
3
6 2 4

```




```input3
2
1 3

```




```output1
YES
1

```




```output2
YES
0

```




```output3
YES
1

```



## Note

<p>In the first example you can simply make one move to obtain sequence <span class="tex-span">[0, 2]</span> with <img align="middle" class="tex-formula" src="file://x6rnrtxE.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second example the <span class="tex-span"><i>gcd</i></span> of the sequence is already greater than <span class="tex-span">1</span>. </p>
