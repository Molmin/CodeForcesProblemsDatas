## Description

<div><p>You have a rooted tree consisting of <span class="tex-span"><i>n</i></span> vertices. Each vertex of the tree has some color. We will assume that the tree vertices are numbered by integers from 1 to <span class="tex-span"><i>n</i></span>. Then we represent the color of vertex <span class="tex-span"><i>v</i></span> as <span class="tex-span"><i>c</i><sub class="lower-index"><i>v</i></sub></span>. The tree root is a vertex with number 1.</p><p>In this problem you need to answer to <span class="tex-span"><i>m</i></span> queries. Each query is described by two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub>, <i>k</i><sub class="lower-index"><i>j</i></sub></span>. The answer to query <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub>, <i>k</i><sub class="lower-index"><i>j</i></sub></span> is the number of such colors of vertices <span class="tex-span"><i>x</i></span>, that the subtree of vertex <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> contains at least <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i></sub></span> vertices of color <span class="tex-span"><i>x</i></span>.</p><p>You can find the definition of a rooted tree by the following link: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Tree_(graph_theory)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains a sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>n</i> - 1</span> lines contain the edges of the tree. The <span class="tex-span"><i>i</i></span>-th line contains the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the vertices connected by an edge of the tree.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the queries. The <span class="tex-span"><i>j</i></span>-th line contains two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub>, <i>k</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>k</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the answers to the queries in the order the queries appear in the input.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains a sequence of integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>n</i> - 1</span> lines contain the edges of the tree. The <span class="tex-span"><i>i</i></span>-th line contains the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the vertices connected by an edge of the tree.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the queries. The <span class="tex-span"><i>j</i></span>-th line contains two integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub>, <i>k</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>k</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the answers to the queries in the order the queries appear in the input.</p>





```input1
8 5
1 2 2 3 3 2 3 3
1 2
1 5
2 3
2 4
5 6
5 7
5 8
1 2
1 3
1 4
2 3
5 3

```




```input2
4 1
1 2 3 4
1 2
2 3
3 4
1 1

```




```output1
2
2
1
0
1

```




```output2
4

```



## Note

<p>A subtree of vertex <span class="tex-span"><i>v</i></span> in a rooted tree with root <span class="tex-span"><i>r</i></span> is a set of vertices <span class="tex-span">{<i>u</i>&nbsp;: <i>dist</i>(<i>r</i>, <i>v</i>) + <i>dist</i>(<i>v</i>, <i>u</i>) = <i>dist</i>(<i>r</i>, <i>u</i>)}</span>. Where <span class="tex-span"><i>dist</i>(<i>x</i>, <i>y</i>)</span> is the length (in edges) of the shortest path between vertices <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p>
