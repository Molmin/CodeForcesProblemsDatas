## Description

<div><p>Sagheer is playing a game with his best friend Soliman. He brought a tree with <span class="tex-span"><i>n</i></span> nodes numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and rooted at node <span class="tex-span">1</span>. The <span class="tex-span"><i>i</i></span>-th node has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> apples. This tree has a special property: the lengths of all paths from the root to any leaf have the same parity (i.e. all paths have even length or all paths have odd length).</p><p>Sagheer and Soliman will take turns to play. Soliman will make the first move. The player who can't make a move loses.</p><p>In each move, the current player will pick a single node, take a non-empty subset of apples from it and do one of the following two things:</p><ol> <li> eat the apples, if the node is a leaf. </li><li> move the apples to one of the children, if the node is non-leaf. </li></ol><p>Before Soliman comes to start playing, Sagheer will make <span class="tex-font-style-bf">exactly one change</span> to the tree. He will pick two different nodes <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> and swap the apples of <span class="tex-span"><i>u</i></span> with the apples of <span class="tex-span"><i>v</i></span>.</p><p>Can you help Sagheer count the number of ways to make the swap (i.e. to choose <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>) after which he will win the game if both players play optimally? <span class="tex-span">(<i>u</i>, <i>v</i>)</span> and <span class="tex-span">(<i>v</i>, <i>u</i>)</span> are considered to be the same pair.</p></div><div class="input-specification"><p>The first line will contain one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes in the apple tree.</p><p>The second line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the number of apples on each node of the tree.</p><p>The third line will contain <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the parent of each node of the tree. Node <span class="tex-span"><i>i</i></span> has parent <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (for <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>). Node <span class="tex-span">1</span> is the root of the tree.</p><p>It is guaranteed that the input describes a valid tree, and the lengths of all paths from the root to any leaf will have the same parity.</p></div><div class="output-specification"><p>On a single line, print the number of different pairs of nodes <span class="tex-span">(<i>u</i>, <i>v</i>)</span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span> such that if they start playing after swapping the apples of both nodes, Sagheer will win the game. <span class="tex-span">(<i>u</i>, <i>v</i>)</span> and <span class="tex-span">(<i>v</i>, <i>u</i>)</span> are considered to be the same pair.</p></div>

## Input

<p>The first line will contain one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes in the apple tree.</p><p>The second line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the number of apples on each node of the tree.</p><p>The third line will contain <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the parent of each node of the tree. Node <span class="tex-span"><i>i</i></span> has parent <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (for <span class="tex-span">2 ≤ <i>i</i> ≤ <i>n</i></span>). Node <span class="tex-span">1</span> is the root of the tree.</p><p>It is guaranteed that the input describes a valid tree, and the lengths of all paths from the root to any leaf will have the same parity.</p>

## Output

<p>On a single line, print the number of different pairs of nodes <span class="tex-span">(<i>u</i>, <i>v</i>)</span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span> such that if they start playing after swapping the apples of both nodes, Sagheer will win the game. <span class="tex-span">(<i>u</i>, <i>v</i>)</span> and <span class="tex-span">(<i>v</i>, <i>u</i>)</span> are considered to be the same pair.</p>





```input1
3
2 2 3
1 1

```




```input2
3
1 2 3
1 1

```




```input3
8
7 2 2 5 4 3 1 1
1 1 1 4 4 5 6

```




```output1
1

```




```output2
0

```




```output3
4

```



## Note

<p>In the first sample, Sagheer can only win if he swapped node <span class="tex-span">1</span> with node <span class="tex-span">3</span>. In this case, both leaves will have <span class="tex-span">2</span> apples. If Soliman makes a move in a leaf node, Sagheer can make the same move in the other leaf. If Soliman moved some apples from a root to a leaf, Sagheer will eat those moved apples. Eventually, Soliman will not find a move.</p><p>In the second sample, There is no swap that will make Sagheer win the game.</p><p>Note that Sagheer must make the swap even if he can win with the initial tree.</p>
