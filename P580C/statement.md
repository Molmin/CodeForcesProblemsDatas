## Description

<div><p>Kefa decided to celebrate his first big salary by going to the restaurant. </p><p>He lives by an unusual park. The park is a rooted tree consisting of <span class="tex-span"><i>n</i></span> vertices with the root at vertex <span class="tex-span">1</span>. Vertex <span class="tex-span">1</span> also contains Kefa's house. Unfortunaely for our hero, the park also contains cats. Kefa has already found out what are the vertices with cats in them.</p><p>The leaf vertices of the park contain restaurants. Kefa wants to choose a restaurant where he will go, but unfortunately he is very afraid of cats, so there is no way he will go to the restaurant if the path from the restaurant to his house contains more than <span class="tex-span"><i>m</i></span> <span class="tex-font-style-bf">consecutive</span> vertices with cats. </p><p>Your task is to help Kefa count the number of restaurants where he can go.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — the number of vertices of the tree and the maximum number of consecutive vertices with cats that is still ok for Kefa.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> either equals to <span class="tex-span">0</span> (then vertex <span class="tex-span"><i>i</i></span> has no cat), or equals to <span class="tex-span">1</span> (then vertex <span class="tex-span"><i>i</i></span> has a cat).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contains the edges of the tree in the format "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes) (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the vertices of the tree, connected by an edge. </p><p>It is guaranteed that the given set of edges specifies a tree.</p></div><div class="output-specification"><p>A single integer — the number of distinct leaves of a tree the path to which from Kefa's home contains at most <span class="tex-span"><i>m</i></span> consecutive vertices with cats.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>) — the number of vertices of the tree and the maximum number of consecutive vertices with cats that is still ok for Kefa.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> either equals to <span class="tex-span">0</span> (then vertex <span class="tex-span"><i>i</i></span> has no cat), or equals to <span class="tex-span">1</span> (then vertex <span class="tex-span"><i>i</i></span> has a cat).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contains the edges of the tree in the format "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>" (without the quotes) (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the vertices of the tree, connected by an edge. </p><p>It is guaranteed that the given set of edges specifies a tree.</p>

## Output

<p>A single integer — the number of distinct leaves of a tree the path to which from Kefa's home contains at most <span class="tex-span"><i>m</i></span> consecutive vertices with cats.</p>





```input1
4 1
1 1 0 0
1 2
1 3
1 4

```




```input2
7 1
1 0 1 1 0 0 0
1 2
1 3
2 4
2 5
3 6
3 7

```




```output1
2

```




```output2
2

```



## Note

<p>Let us remind you that a <span class="tex-font-style-it">tree</span> is a connected graph on <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>n</i> - 1</span> edge. A <span class="tex-font-style-it">rooted</span> tree is a tree with a special vertex called <span class="tex-font-style-it">root</span>. In a rooted tree among any two vertices connected by an edge, one vertex is a parent (the one closer to the root), and the other one is a child. A vertex is called a <span class="tex-font-style-it">leaf</span>, if it has no children.</p><p>Note to the first sample test: <img class="tex-graphics" src="file://YAIUSMsI.png" style="max-width: 100.0%;max-height: 100.0%;"> The vertices containing cats are marked red. The restaurants are at vertices 2, 3, 4. Kefa can't go only to the restaurant located at vertex <span class="tex-span">2</span>.</p><p>Note to the second sample test: <img class="tex-graphics" src="file://O8I7s07y.png" style="max-width: 100.0%;max-height: 100.0%;"> The restaurants are located at vertices 4, 5, 6, 7. Kefa can't go to restaurants 6, 7.</p>
