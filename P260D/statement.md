## Description

<div><p>The board has got a painted tree graph, consisting of <span class="tex-span"><i>n</i></span> nodes. Let us remind you that a non-directed graph is called a tree if it is connected and doesn't contain any cycles.</p><p>Each node of the graph is painted black or white in such a manner that there aren't two nodes of the same color, connected by an edge. Each edge contains its value written on it as a non-negative integer.</p><p>A bad boy Vasya came up to the board and wrote number <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span> near each node <span class="tex-span"><i>v</i></span> — the sum of values of all edges that are incident to this node. Then Vasya removed the edges and their values from the board.</p><p>Your task is to restore the original tree by the node colors and numbers <span class="tex-span"><i>s</i><sub class="lower-index"><i>v</i></sub></span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of nodes in the tree. Next <span class="tex-span"><i>n</i></span> lines contain pairs of space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> stands for the color of the <span class="tex-span"><i>i</i></span>-th vertex (0 is for white, 1 is for black), and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> represents the sum of values of the edges that are incident to the <span class="tex-span"><i>i</i></span>-th vertex of the tree that is painted on the board.</p></div><div class="output-specification"><p>Print the description of <span class="tex-span"><i>n</i> - 1</span> edges of the tree graph. Each description is a group of three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> — are the numbers of the nodes that are connected by the <span class="tex-span"><i>i</i></span>-th edge, and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is its value. Note that the following condition must fulfill <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i><sub class="lower-index"><i>i</i></sub></sub> ≠ <i>c</i><sub class="lower-index"><i>u</i><sub class="lower-index"><i>i</i></sub></sub></span>.</p><p>It is guaranteed that for any input data there exists at least one graph that meets these data. If there are multiple solutions, print any of them. You are allowed to print the edges in any order. As you print the numbers, separate them with spaces.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of nodes in the tree. Next <span class="tex-span"><i>n</i></span> lines contain pairs of space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> stands for the color of the <span class="tex-span"><i>i</i></span>-th vertex (0 is for white, 1 is for black), and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> represents the sum of values of the edges that are incident to the <span class="tex-span"><i>i</i></span>-th vertex of the tree that is painted on the board.</p>

## Output

<p>Print the description of <span class="tex-span"><i>n</i> - 1</span> edges of the tree graph. Each description is a group of three integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> — are the numbers of the nodes that are connected by the <span class="tex-span"><i>i</i></span>-th edge, and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is its value. Note that the following condition must fulfill <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i><sub class="lower-index"><i>i</i></sub></sub> ≠ <i>c</i><sub class="lower-index"><i>u</i><sub class="lower-index"><i>i</i></sub></sub></span>.</p><p>It is guaranteed that for any input data there exists at least one graph that meets these data. If there are multiple solutions, print any of them. You are allowed to print the edges in any order. As you print the numbers, separate them with spaces.</p>





```input1
3
1 3
1 2
0 5

```




```input2
6
1 0
0 3
1 8
0 2
0 3
0 0

```




```output1
3 1 3
3 2 2

```




```output2
2 3 3
5 3 3
4 3 2
1 6 0
2 1 0

```


