## Description

<div><p>In computer science, there is a method called "Divide And Conquer By Node" to solve some hard problems about paths on a tree. Let's desribe how this method works by function:</p><p><span class="tex-span"><i>solve</i>(<i>t</i>)</span> (<span class="tex-span"><i>t</i></span> is a tree): </p><ol> <li> Chose a node <span class="tex-span"><i>x</i></span> (it's common to chose weight-center) in tree <span class="tex-span"><i>t</i></span>. Let's call this step "Line A". </li><li> Deal with all paths that pass <span class="tex-span"><i>x</i></span>. </li><li> Then delete <span class="tex-span"><i>x</i></span> from tree <span class="tex-span"><i>t</i></span>. </li><li> After that <span class="tex-span"><i>t</i></span> becomes some subtrees. </li><li> Apply <span class="tex-span"><i>solve</i></span> on each subtree. </li></ol><p>This ends when <span class="tex-span"><i>t</i></span> has only one node because after deleting it, there's nothing. </p><p>Now, WJMZBMR has mistakenly believed that it's ok to chose any node in "Line A". So he'll chose a node at random. To make the situation worse, he thinks a "tree" should have the same number of edges and nodes! So this procedure becomes like that.</p><p>Let's define the variable <span class="tex-span"><i>totalCost</i></span>. Initially the value of <span class="tex-span"><i>totalCost</i></span> equal to <span class="tex-span">0</span>. So, <span class="tex-span"><i>solve</i>(<i>t</i>)</span> (now <span class="tex-span"><i>t</i></span> is a graph): </p><ol> <li> <span class="tex-span"><i>totalCost</i> = <i>totalCost</i> + (<i>size</i>&nbsp;<i>of</i>&nbsp;<i>t</i>)</span>. The operation "<span class="tex-font-style-tt">=</span>" means assignment. <span class="tex-span">(<i>Size</i>&nbsp;<i>of</i>&nbsp;<i>t</i>)</span> means the number of nodes in <span class="tex-span"><i>t</i></span>. </li><li> Choose a node <span class="tex-span"><i>x</i></span> in graph <span class="tex-span"><i>t</i></span> at random (uniformly among all nodes of <span class="tex-span"><i>t</i></span>). </li><li> Then delete <span class="tex-span"><i>x</i></span> from graph <span class="tex-span"><i>t</i></span>. </li><li> After that <span class="tex-span"><i>t</i></span> becomes some connected components. </li><li> Apply <span class="tex-span"><i>solve</i></span> on each component. </li></ol><p>He'll apply <span class="tex-span"><i>solve</i></span> on a connected graph with <span class="tex-span"><i>n</i></span> nodes and <span class="tex-span"><i>n</i></span> edges. He thinks it will work quickly, but it's very slow. So he wants to know the expectation of <span class="tex-span"><i>totalCost</i></span> of this procedure. Can you help him?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>) — the number of nodes and edges in the graph. Each of the next <span class="tex-span"><i>n</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1)</span> indicating an edge between nodes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider that the graph nodes are numbered from <span class="tex-span">0</span> to <span class="tex-span">(<i>n</i> - 1)</span>. It's guaranteed that there are no self-loops, no multiple edges in that graph. It's guaranteed that the graph is connected.</p></div><div class="output-specification"><p>Print a single real number — the expectation of <span class="tex-span"><i>totalCost</i></span>. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3000</span>) — the number of nodes and edges in the graph. Each of the next <span class="tex-span"><i>n</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1)</span> indicating an edge between nodes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Consider that the graph nodes are numbered from <span class="tex-span">0</span> to <span class="tex-span">(<i>n</i> - 1)</span>. It's guaranteed that there are no self-loops, no multiple edges in that graph. It's guaranteed that the graph is connected.</p>

## Output

<p>Print a single real number — the expectation of <span class="tex-span"><i>totalCost</i></span>. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
5
3 4
2 3
2 4
0 4
1 2

```




```input2
3
0 1
1 2
0 2

```




```input3
5
0 1
1 2
2 0
3 0
4 1

```




```output1
13.166666666666666

```




```output2
6.000000000000000

```




```output3
13.166666666666666

```



## Note

<p>Consider the second example. No matter what we choose first, the <span class="tex-span"><i>totalCost</i></span> will always be <span class="tex-span">3 + 2 + 1 = 6</span>.</p>
