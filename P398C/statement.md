## Description

<div><p>User ainta likes trees. This time he is going to make an undirected tree with <span class="tex-span"><i>n</i></span> vertices numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The tree is weighted, so each edge of the tree will have some integer weight.</p><p>Also he has an array <span class="tex-span"><i>t</i></span>: <span class="tex-span"><i>t</i>[1], <i>t</i>[2], ..., <i>t</i>[<i>n</i>]</span>. At first all the elements of the array are initialized to <span class="tex-span">0</span>. Then for each edge connecting vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>u</i> &lt; <i>v</i></span>) of the tree with weight <span class="tex-span"><i>c</i></span>, ainta adds value <span class="tex-span"><i>c</i></span> to the elements <span class="tex-span"><i>t</i>[<i>u</i>], <i>t</i>[<i>u</i> + 1], ..., <i>t</i>[<i>v</i> - 1], <i>t</i>[<i>v</i>]</span> of array <span class="tex-span"><i>t</i></span>.</p><p>Let's assume that <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> is the total weight of edges on the shortest path between vertex <span class="tex-span"><i>u</i></span> and vertex <span class="tex-span"><i>v</i></span>. User ainta calls a pair of integers <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> &lt; <i>y</i> ≤ <i>n</i></span>) <span class="tex-font-style-it">good</span> if and only if <span class="tex-span"><i>d</i>(<i>x</i>, <i>y</i>) = <i>t</i>[<i>x</i>] + <i>t</i>[<i>x</i> + 1] + ... + <i>t</i>[<i>y</i> - 1] + <i>t</i>[<i>y</i>]</span>.</p><p>User ainta wants to make at least <img align="middle" class="tex-formula" src="file://CDn7s5pd.png" style="max-width: 100.0%;max-height: 100.0%;"> good pairs, but he couldn't make a proper tree. Help ainta to find such a tree.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i> - 1</span> lines containing the description of the edges. The <span class="tex-span"><i>i</i></span>-th line should contain three space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> &lt; <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — two vertices connected by the edge, and the weight of the edge.</p><p>Next print <img align="middle" class="tex-formula" src="file://Q70CbdwJ.png" style="max-width: 100.0%;max-height: 100.0%;"> lines containing the good pairs. The <span class="tex-span"><i>k</i></span>-th line should contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>k</i></sub> &lt; <i>y</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>). Of course, <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span> must be a good pair. All pairs should be distinct — that is, for all <span class="tex-span"><i>j</i>, <i>k</i></span> <img align="middle" class="tex-formula" src="file://DdhhPmez.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> ≠ <i>x</i><sub class="lower-index"><i>k</i></sub></span> or <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub> ≠ <i>y</i><sub class="lower-index"><i>k</i></sub></span> must be satisfied.</p><p>If there are many correct solutions, print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i> - 1</span> lines containing the description of the edges. The <span class="tex-span"><i>i</i></span>-th line should contain three space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub> &lt; <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — two vertices connected by the edge, and the weight of the edge.</p><p>Next print <img align="middle" class="tex-formula" src="file://Q70CbdwJ.png" style="max-width: 100.0%;max-height: 100.0%;"> lines containing the good pairs. The <span class="tex-span"><i>k</i></span>-th line should contain two space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>k</i></sub> &lt; <i>y</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>). Of course, <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub>, <i>y</i><sub class="lower-index"><i>k</i></sub></span> must be a good pair. All pairs should be distinct — that is, for all <span class="tex-span"><i>j</i>, <i>k</i></span> <img align="middle" class="tex-formula" src="file://DdhhPmez.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> ≠ <i>x</i><sub class="lower-index"><i>k</i></sub></span> or <span class="tex-span"><i>y</i><sub class="lower-index"><i>j</i></sub> ≠ <i>y</i><sub class="lower-index"><i>k</i></sub></span> must be satisfied.</p><p>If there are many correct solutions, print any of them.</p>





```input1
7
```




```output1
1 4 1
1 2 2
2 3 5
3 5 3
2 6 2
6 7 3
4 5
5 6
5 7
```



## Note

<p><span class="tex-span">⌊<i>x</i>⌋</span> is the largest integer not greater than <span class="tex-span"><i>x</i></span>.</p><p>You can find the definition of a tree by the following link: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Tree_(graph_theory)</span></p><p>You can also find the definition of the shortest path by the following link: <span class="tex-font-style-tt">http://en.wikipedia.org/wiki/Shortest_path_problem</span></p><p>The tree and the array <span class="tex-span"><i>t</i></span> in the sample output look like this:</p><center> <img class="tex-graphics" src="file://FBgknWEa.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
