## Description

<div><p>Momiji has got a rooted tree, consisting of <span class="tex-span"><i>n</i></span> nodes. The tree nodes are numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The root has number <span class="tex-span">1</span>. Momiji decided to play a game on this tree.</p><p>The game consists of several steps. On each step, Momiji chooses one of the remaining tree nodes (let's denote it by <span class="tex-span"><i>v</i></span>) and removes all the subtree nodes with the root in node <span class="tex-span"><i>v</i></span> from the tree. Node <span class="tex-span"><i>v</i></span> gets deleted as well. The game finishes when the tree has no nodes left. In other words, the game finishes after the step that chooses the node number <span class="tex-span">1</span>.</p><p>Each time Momiji chooses a new node uniformly among all the remaining nodes. Your task is to find the expectation of the number of steps in the described game.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes in the tree. The next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers of the nodes that are connected by the <span class="tex-span"><i>i</i></span>-th edge.</p><p>It is guaranteed that the given graph is a tree.</p></div><div class="output-specification"><p>Print a single real number — the expectation of the number of steps in the described game.</p><p>The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes in the tree. The next <span class="tex-span"><i>n</i> - 1</span> lines contain the tree edges. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers of the nodes that are connected by the <span class="tex-span"><i>i</i></span>-th edge.</p><p>It is guaranteed that the given graph is a tree.</p>

## Output

<p>Print a single real number — the expectation of the number of steps in the described game.</p><p>The answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2
1 2

```




```input2
3
1 2
1 3

```




```output1
1.50000000000000000000

```




```output2
2.00000000000000000000

```



## Note

<p>In the first sample, there are two cases. One is directly remove the root and another is remove the root after one step. Thus the expected steps are: </p><center class="tex-equation"><span class="tex-span">1 × (1 / 2) + 2 × (1 / 2) = 1.5</span></center><p>In the second sample, things get more complex. There are two cases that reduce to the first sample, and one case cleaned at once. Thus the expected steps are: </p><center class="tex-equation"><span class="tex-span">1 × (1 / 3) + (1 + 1.5) × (2 / 3) = (1 / 3) + (5 / 3) = 2</span></center>
