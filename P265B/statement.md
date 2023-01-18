## Description

<div><p>Squirrel Liss loves nuts. There are <span class="tex-span"><i>n</i></span> trees (numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from west to east) along a street and there is a delicious nut on the top of each tree. The height of the tree <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Liss wants to eat all nuts.</p><p>Now Liss is on the root of the tree with the number <span class="tex-span">1</span>. In one second Liss can perform one of the following actions:</p><ul> <li> Walk up or down one unit on a tree. </li><li> Eat a nut on the top of the current tree. </li><li> Jump to the next tree. In this action the height of Liss doesn't change. More formally, when Liss is at height <span class="tex-span"><i>h</i></span> of the tree <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>), she jumps to height <span class="tex-span"><i>h</i></span> of the tree <span class="tex-span"><i>i</i> + 1</span>. This action can't be performed if <span class="tex-span"><i>h</i> &gt; <i>h</i><sub class="lower-index"><i>i</i> + 1</sub></span>. </li></ul><p>Compute the minimal time (in seconds) required to eat all nuts.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of trees.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains the height of trees: <span class="tex-span"><i>i</i></span>-th line contains an integer <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the height of the tree with the number <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print a single integer — the minimal time required to eat all nuts in seconds.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of trees.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains the height of trees: <span class="tex-span"><i>i</i></span>-th line contains an integer <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the height of the tree with the number <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print a single integer — the minimal time required to eat all nuts in seconds.</p>





```input1
2
1
2

```




```input2
5
2
1
2
1
1

```




```output1
5

```




```output2
14

```


