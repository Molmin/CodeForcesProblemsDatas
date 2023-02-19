## Description

<div><p>Given a rooted tree with <span class="tex-span"><i>n</i></span> nodes. The Night King removes exactly one node from the tree and all the edges associated with it. Doing this splits the tree and forms a forest. The node which is removed is not a part of the forest.</p><p>The root of a tree in the forest is the node in that tree which does not have a parent. We define the strength of the forest as the size of largest tree in forest.</p><p>Jon Snow wants to minimize the strength of the forest. To do this he can perform the following operation at most once.</p><p><span class="tex-font-style-it">He removes the edge between a node and its parent and inserts a new edge between this node and any other node in forest such that the total number of trees in forest remain same.</span></p><p>For each node <span class="tex-span"><i>v</i></span> you need to find the minimum value of strength of the forest formed when node <span class="tex-span"><i>v</i></span> is removed.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree. Each of the next <span class="tex-span"><i>n</i></span> lines contains a pair of vertex indices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i></span>) where <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the parent of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> = 0</span> then <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the root.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> line each containing a single integer. The <span class="tex-span"><i>i</i></span>-th of them should be equal to minimum value of strength of forest formed when <span class="tex-span"><i>i</i></span>-th node is removed and Jon Snow performs the operation described above at most once.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree. Each of the next <span class="tex-span"><i>n</i></span> lines contains a pair of vertex indices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤  <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub>  ≤  <i>n</i></span>) where <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> is the parent of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> = 0</span> then <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the root.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> line each containing a single integer. The <span class="tex-span"><i>i</i></span>-th of them should be equal to minimum value of strength of forest formed when <span class="tex-span"><i>i</i></span>-th node is removed and Jon Snow performs the operation described above at most once.</p>





```input1
10
0 1
1 2
1 3
1 4
2 5
2 6
3 7
4 8
4 9
5 10

```




```input2
2
2 1
0 2

```




```output1
3
4
5
5
5
9
9
9
9
9

```




```output2
1
1

```



## Note

<p>The tree for first test case is depicted below. <img class="tex-graphics" src="file://tkq6rxUK.png" style="max-width: 100.0%;max-height: 100.0%;"> When you remove the first node, the tree splits to form the following forest. The strength of this forest is <span class="tex-span">4</span>. <img class="tex-graphics" src="file://Ji3d9WpS.png" style="max-width: 100.0%;max-height: 100.0%;"> Jon Snow now changes the parent of vertex <span class="tex-span">10</span> from <span class="tex-span">5</span> to <span class="tex-span">3</span>. The strength of forest now becomes <span class="tex-span">3</span>. <img class="tex-graphics" src="file://OV0SHkry.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
