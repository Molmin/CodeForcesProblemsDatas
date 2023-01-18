## Description

<div><p>You have two rooted undirected trees, each contains <span class="tex-span"><i>n</i></span> vertices. Let's number the vertices of each tree with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The root of each tree is at vertex <span class="tex-span">1</span>. The edges of the first tree are painted blue, the edges of the second one are painted red. For simplicity, let's say that the first tree is blue and the second tree is red.</p><p>Edge <span class="tex-span">{<i>x</i>, <i>y</i>}</span> is called bad for edge <span class="tex-span">{<i>p</i>, <i>q</i>}</span> if two conditions are fulfilled: </p><ol> <li> The color of edge <span class="tex-span">{<i>x</i>, <i>y</i>}</span> is different from the color of edge <span class="tex-span">{<i>p</i>, <i>q</i>}</span>. </li><li> Let's consider the tree of the same color that edge <span class="tex-span">{<i>p</i>, <i>q</i>}</span> is. Exactly one of vertices <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> lies both in the subtree of vertex <span class="tex-span"><i>p</i></span> and in the subtree of vertex <span class="tex-span"><i>q</i></span>. </li></ol><p>In this problem, your task is to simulate the process described below. The process consists of several stages:</p><ol> <li> On each stage edges of exactly one color are deleted. </li><li> On the first stage, exactly one blue edge is deleted. </li><li> Let's assume that at the stage <span class="tex-span"><i>i</i></span> we've deleted edges <span class="tex-span">{<i>u</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">1</sub>}</span>, <span class="tex-span">{<i>u</i><sub class="lower-index">2</sub>, <i>v</i><sub class="lower-index">2</sub>}</span>, <span class="tex-span">...</span>, <span class="tex-span">{<i>u</i><sub class="lower-index"><i>k</i></sub>, <i>v</i><sub class="lower-index"><i>k</i></sub>}</span>. At the stage <span class="tex-span"><i>i</i> + 1</span> we will delete all undeleted bad edges for edge <span class="tex-span">{<i>u</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">1</sub>}</span>, then we will delete all undeleted bad edges for edge <span class="tex-span">{<i>u</i><sub class="lower-index">2</sub>, <i>v</i><sub class="lower-index">2</sub>}</span> and so on until we reach edge <span class="tex-span">{<i>u</i><sub class="lower-index"><i>k</i></sub>, <i>v</i><sub class="lower-index"><i>k</i></sub>}</span>. </li></ol> <p>For each stage of deleting edges determine what edges will be removed on the stage. Note that the definition of a bad edge always considers the initial tree before it had any edges removed.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of vertices in each tree.</p><p>The next line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>) — the description of edges of the first tree. Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means that the first tree has an edge connecting vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and vertex <span class="tex-span"><i>i</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">3</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>) — the description of the edges of the second tree. Number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> means that the second tree has an edge connecting vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and vertex <span class="tex-span"><i>i</i></span>. </p><p>The next line contains integer <span class="tex-span"><i>idx</i></span> (<span class="tex-span">1 ≤ <i>idx</i> &lt; <i>n</i></span>) — the index of the blue edge that was removed on the first stage. Assume that the edges of each tree are numbered with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> in the order in which they are given in the input. </p></div><div class="output-specification"><p>For each stage of removing edges print its description. Each description must consist of exactly two lines. If this is the stage when blue edges are deleted, then the first line of the description must contain word <span class="tex-span"><i>Blue</i></span>, otherwise — word <span class="tex-span"><i>Red</i></span>. In the second line print the indexes of the edges that will be deleted on this stage in the increasing order.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of vertices in each tree.</p><p>The next line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>) — the description of edges of the first tree. Number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means that the first tree has an edge connecting vertex <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and vertex <span class="tex-span"><i>i</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">3</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>b</i><sub class="lower-index"><i>i</i></sub> ≠ <i>i</i></span>) — the description of the edges of the second tree. Number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> means that the second tree has an edge connecting vertex <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and vertex <span class="tex-span"><i>i</i></span>. </p><p>The next line contains integer <span class="tex-span"><i>idx</i></span> (<span class="tex-span">1 ≤ <i>idx</i> &lt; <i>n</i></span>) — the index of the blue edge that was removed on the first stage. Assume that the edges of each tree are numbered with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> in the order in which they are given in the input. </p>

## Output

<p>For each stage of removing edges print its description. Each description must consist of exactly two lines. If this is the stage when blue edges are deleted, then the first line of the description must contain word <span class="tex-span"><i>Blue</i></span>, otherwise — word <span class="tex-span"><i>Red</i></span>. In the second line print the indexes of the edges that will be deleted on this stage in the increasing order.</p>





```input1
5
1 1 1 1
4 2 1 1
3

```




```output1
Blue
3
Red
1 3
Blue
1 2
Red
2

```



## Note

<p>For simplicity let's assume that all edges of the root tree received some direction, so that all vertices are reachable from vertex <span class="tex-span">1</span>. Then a <span class="tex-font-style-it">subtree</span> of vertex <span class="tex-span"><i>v</i></span> is a set of vertices reachable from vertex <span class="tex-span"><i>v</i></span> in the resulting directed graph (vertex <span class="tex-span"><i>v</i></span> is also included in the set).</p>
