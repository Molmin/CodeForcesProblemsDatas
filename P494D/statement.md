## Description

<div><p>Ali is Hamed's little brother and tomorrow is his birthday. Hamed wants his brother to earn his gift so he gave him a hard programming problem and told him if he can successfully solve it, he'll get him a brand new laptop. Ali is not yet a very talented programmer like Hamed and although he usually doesn't cheat but this time is an exception. It's about a brand new laptop. So he decided to secretly seek help from you. Please solve this problem for Ali. </p><p>An <span class="tex-span"><i>n</i></span>-vertex weighted rooted tree is given. Vertex number <span class="tex-span">1</span> is a root of the tree. We define <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> as the sum of edges weights on the shortest path between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. Specifically we define <span class="tex-span"><i>d</i>(<i>u</i>, <i>u</i>) = 0</span>. Also let's define <span class="tex-span"><i>S</i>(<i>v</i>)</span> for each vertex <span class="tex-span"><i>v</i></span> as a set containing all vertices <span class="tex-span"><i>u</i></span> such that <span class="tex-span"><i>d</i>(1, <i>u</i>) = <i>d</i>(1, <i>v</i>) + <i>d</i>(<i>v</i>, <i>u</i>)</span>. Function <span class="tex-span"><i>f</i>(<i>u</i>, <i>v</i>)</span> is then defined using the following formula:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://kFYoM75h.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The goal is to calculate <span class="tex-span"><i>f</i>(<i>u</i>, <i>v</i>)</span> for each of the <span class="tex-span"><i>q</i></span> given pair of vertices. As the answer can be rather large it's enough to print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>In the first line of input an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), number of vertices of the tree is given.</p><p>In each of the next <span class="tex-span"><i>n</i> - 1</span> lines three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given indicating an edge between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with weight equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>In the next line an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), number of vertex pairs, is given.</p><p>In each of the next <span class="tex-span"><i>q</i></span> lines two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) are given meaning that you must calculate <span class="tex-span"><i>f</i>(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the value of <span class="tex-span"><i>f</i>(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>In the first line of input an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), number of vertices of the tree is given.</p><p>In each of the next <span class="tex-span"><i>n</i> - 1</span> lines three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) are given indicating an edge between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with weight equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>In the next line an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), number of vertex pairs, is given.</p><p>In each of the next <span class="tex-span"><i>q</i></span> lines two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) are given meaning that you must calculate <span class="tex-span"><i>f</i>(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>It is guaranteed that the given edges form a tree.</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print the value of <span class="tex-span"><i>f</i>(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>)</span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
5
1 2 1
4 3 1
3 5 1
1 3 1
5
1 1
1 5
2 4
2 1
3 5

```




```input2
8
1 2 100
1 3 20
2 4 2
2 5 1
3 6 1
3 7 2
6 8 5
6
1 8
2 3
5 8
2 6
4 7
6 1

```




```output1
10
1000000005
1000000002
23
1000000002

```




```output2
999968753
49796
999961271
999991235
999958569
45130

```


