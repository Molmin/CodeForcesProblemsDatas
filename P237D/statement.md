## Description

<div><p>You've got a undirected tree <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> nodes. Your task is to build an optimal T-decomposition for it. Let's define a T-decomposition as follows.</p><p>Let's denote the set of all nodes <span class="tex-span"><i>s</i></span> as <span class="tex-span"><i>v</i></span>. Let's consider an undirected tree <span class="tex-span"><i>t</i></span>, whose nodes are some non-empty subsets of <span class="tex-span"><i>v</i></span>, we'll call them <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <img align="middle" class="tex-formula" src="file://megzWntA.png" style="max-width: 100.0%;max-height: 100.0%;">. The tree <span class="tex-span"><i>t</i></span> is a T-decomposition of <span class="tex-span"><i>s</i></span>, if the following conditions holds:</p><ol> <li> the union of all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span"><i>v</i></span>; </li><li> for any edge <span class="tex-span">(<i>a</i>, <i>b</i>)</span> of tree <span class="tex-span"><i>s</i></span> exists the tree node <span class="tex-span"><i>t</i></span>, containing both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>; </li><li> if the nodes of the tree <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> contain the node <span class="tex-span"><i>a</i></span> of the tree <span class="tex-span"><i>s</i></span>, then all nodes of the tree <span class="tex-span"><i>t</i></span>, lying on the path from <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> also contain node <span class="tex-span"><i>a</i></span>. So this condition is equivalent to the following: all nodes of the tree <span class="tex-span"><i>t</i></span>, that contain node <span class="tex-span"><i>a</i></span> of the tree <span class="tex-span"><i>s</i></span>, form a connected subtree of tree <span class="tex-span"><i>t</i></span>. </li></ol><p>There are obviously many distinct trees <span class="tex-span"><i>t</i></span>, that are T-decompositions of the tree <span class="tex-span"><i>s</i></span>. For example, a T-decomposition is a tree that consists of a single node, equal to set <span class="tex-span"><i>v</i></span>.</p><p>Let's define the cardinality of node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> as the number of nodes in tree <span class="tex-span"><i>s</i></span>, containing in the node. Let's choose the node with the maximum cardinality in <span class="tex-span"><i>t</i></span>. Let's assume that its cardinality equals <span class="tex-span"><i>w</i></span>. Then the weight of T-decomposition <span class="tex-span"><i>t</i></span> is value <span class="tex-span"><i>w</i></span>. The optimal T-decomposition is the one with the minimum weight.</p><p>Your task is to find the optimal T-decomposition of the given tree <span class="tex-span"><i>s</i></span> that has the minimum number of nodes.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, that denotes the number of nodes in tree <span class="tex-span"><i>s</i></span>.</p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting that the nodes of tree <span class="tex-span"><i>s</i></span> with indices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are connected by an edge.</p><p>Consider the nodes of tree <span class="tex-span"><i>s</i></span> indexed from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that <span class="tex-span"><i>s</i></span> is a tree.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>m</i></span> that denotes the number of nodes in the required T-decomposition.</p><p>Then print <span class="tex-span"><i>m</i></span> lines, containing descriptions of the T-decomposition nodes. In the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>m</i>)</span> of them print the description of node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> of the T-decomposition. The description of each node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> should start from an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, that represents the number of nodes of the initial tree <span class="tex-span"><i>s</i></span>, that are contained in the node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Then you should print <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers — the numbers of nodes from <span class="tex-span"><i>s</i></span>, contained in <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, in arbitrary order.</p><p>Then print <span class="tex-span"><i>m</i> - 1</span> lines, each consisting two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>;&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>q</i><sub class="lower-index"><i>i</i></sub>)</span>. The pair of integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></span> means there is an edge between nodes <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sub></span> of T-decomposition.</p><p>The printed T-decomposition should be the optimal T-decomposition for the given tree <span class="tex-span"><i>s</i></span> and have the minimum possible number of nodes among all optimal T-decompositions. If there are multiple optimal T-decompositions with the minimum number of nodes, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, that denotes the number of nodes in tree <span class="tex-span"><i>s</i></span>.</p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, denoting that the nodes of tree <span class="tex-span"><i>s</i></span> with indices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are connected by an edge.</p><p>Consider the nodes of tree <span class="tex-span"><i>s</i></span> indexed from 1 to <span class="tex-span"><i>n</i></span>. It is guaranteed that <span class="tex-span"><i>s</i></span> is a tree.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>m</i></span> that denotes the number of nodes in the required T-decomposition.</p><p>Then print <span class="tex-span"><i>m</i></span> lines, containing descriptions of the T-decomposition nodes. In the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>m</i>)</span> of them print the description of node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> of the T-decomposition. The description of each node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> should start from an integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>, that represents the number of nodes of the initial tree <span class="tex-span"><i>s</i></span>, that are contained in the node <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Then you should print <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct space-separated integers — the numbers of nodes from <span class="tex-span"><i>s</i></span>, contained in <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, in arbitrary order.</p><p>Then print <span class="tex-span"><i>m</i> - 1</span> lines, each consisting two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>;&nbsp;<i>p</i><sub class="lower-index"><i>i</i></sub> ≠ <i>q</i><sub class="lower-index"><i>i</i></sub>)</span>. The pair of integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>q</i><sub class="lower-index"><i>i</i></sub></span> means there is an edge between nodes <span class="tex-span"><i>x</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>i</i></sub></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>q</i><sub class="lower-index"><i>i</i></sub></sub></span> of T-decomposition.</p><p>The printed T-decomposition should be the optimal T-decomposition for the given tree <span class="tex-span"><i>s</i></span> and have the minimum possible number of nodes among all optimal T-decompositions. If there are multiple optimal T-decompositions with the minimum number of nodes, print any of them.</p>





```input1
2
1 2

```




```input2
3
1 2
2 3

```




```input3
4
2 1
3 1
4 1

```




```output1
1
2 1 2

```




```output2
2
2 1 2
2 2 3
1 2

```




```output3
3
2 2 1
2 3 1
2 4 1
1 2
2 3

```


