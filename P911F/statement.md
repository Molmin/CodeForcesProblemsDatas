## Description

<div><p>You are given an unweighted tree with <span class="tex-span"><i>n</i></span> vertices. Then <span class="tex-span"><i>n</i> - 1</span> following operations are applied to the tree. A single operation consists of the following steps: </p><ol> <li> choose two leaves; </li><li> add the length of the simple path between them to the answer; </li><li> remove one of the chosen leaves from the tree. </li></ol><p>Initial answer (before applying operations) is <span class="tex-span">0</span>. Obviously after <span class="tex-span"><i>n</i> - 1</span> such operations the tree will consist of a single vertex. </p><p>Calculate the maximal possible answer you can achieve, and construct a sequence of operations that allows you to achieve this answer!</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree. </p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the edges of the tree in form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that given graph is a tree.</p></div><div class="output-specification"><p>In the first line print one integer number — maximal possible answer. </p><p>In the next <span class="tex-span"><i>n</i> - 1</span> lines print the operations in order of their applying in format <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> — pair of the leaves that are chosen in the current operation (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub></span> or <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — choosen leaf that is removed from the tree in the current operation. </p><p>See the examples for better understanding.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree. </p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the edges of the tree in form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that given graph is a tree.</p>

## Output

<p>In the first line print one integer number — maximal possible answer. </p><p>In the next <span class="tex-span"><i>n</i> - 1</span> lines print the operations in order of their applying in format <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> — pair of the leaves that are chosen in the current operation (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub></span> or <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — choosen leaf that is removed from the tree in the current operation. </p><p>See the examples for better understanding.</p>





```input1
3
1 2
1 3

```




```input2
5
1 2
1 3
2 4
2 5

```




```output1
3
2 3 3
2 1 1

```




```output2
9
3 5 5
4 3 3
4 1 1
4 2 2

```


