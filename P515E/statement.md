## Description

<div><p>Drazil is a monkey. He lives in a circular park. There are <span class="tex-span"><i>n</i></span> trees around the park. The distance between the <span class="tex-span"><i>i</i></span>-th tree and (<span class="tex-span"><i>i</i> + 1</span>)-st trees is <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, the distance between the <span class="tex-span"><i>n</i></span>-th tree and the first tree is <span class="tex-span"><i>d</i><sub class="lower-index"><i>n</i></sub></span>. The height of the <span class="tex-span"><i>i</i></span>-th tree is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Drazil starts each day with the <span class="tex-font-style-it">morning run</span>. The morning run consists of the following steps:</p><ul> <li> Drazil chooses two different trees </li><li> He starts with climbing up the first tree </li><li> Then he climbs down the first tree, runs around the park (in one of two possible directions) to the second tree, and climbs on it </li><li> Then he finally climbs down the second tree. </li></ul><p>But there are always children playing around some consecutive trees. Drazil can't stand children, so he can't choose the trees close to children. He even can't stay close to those trees.</p><p>If the two trees Drazil chooses are <span class="tex-span"><i>x</i></span>-th and <span class="tex-span"><i>y</i></span>-th, we can estimate the energy the <span class="tex-font-style-it">morning run</span> takes to him as <span class="tex-span">2(<i>h</i><sub class="lower-index"><i>x</i></sub> + <i>h</i><sub class="lower-index"><i>y</i></sub>) + <i>dist</i>(<i>x</i>, <i>y</i>)</span>. Since there are children on exactly one of two arcs connecting <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, the distance <span class="tex-span"><i>dist</i>(<i>x</i>, <i>y</i>)</span> between trees <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> is uniquely defined.</p><p>Now, you know that on the <span class="tex-span"><i>i</i></span>-th day children play between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th tree and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th tree. More formally, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, children play around the trees with indices from range <span class="tex-span">[<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>]</span>, otherwise they play around the trees with indices from <img align="middle" class="tex-formula" src="file://sdmsvXCY.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Please help Drazil to determine which two trees he should choose in order to consume the most energy (since he wants to become fit and cool-looking monkey) and report the resulting amount of energy for each day.</p></div><div class="input-specification"><p>The first line contains two integer <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting number of trees and number of days, respectively. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the distances between consecutive trees.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the heights of trees.</p><p>Each of following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing each new day. There are always at least two different trees Drazil can choose that are not affected by children.</p></div><div class="output-specification"><p>For each day print the answer in a separate line.</p></div>

## Input

<p>The first line contains two integer <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting number of trees and number of days, respectively. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub>, ..., <i>d</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the distances between consecutive trees.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the heights of trees.</p><p>Each of following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing each new day. There are always at least two different trees Drazil can choose that are not affected by children.</p>

## Output

<p>For each day print the answer in a separate line.</p>





```input1
5 3
2 2 2 2 2
3 5 2 1 4
1 3
2 2
4 5

```




```input2
3 3
5 1 4
5 1 4
3 3
2 2
1 1

```




```output1
12
16
18

```




```output2
17
22
11

```


