## Description

<div><p>You are given a tree that has <span class="tex-span"><i>n</i></span> vertices, which are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, where the vertex number one is the root. Each edge has weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and strength <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Botanist Innokentiy, who is the only member of the jury of the Olympiad in Informatics, doesn't like broken trees. </p><p>The tree is broken if there is such an edge the strength of which is less than the sum of weight of subtree's edges to which it leads.</p><p>It is allowed to reduce weight of any edge by arbitrary integer value, but then the strength of its edge is reduced by the same value. It means if the weight of the edge is <span class="tex-span">10</span>, and the strength is <span class="tex-span">12</span>, then by the reducing the weight by <span class="tex-span">7</span> its weight will equal <span class="tex-span">3</span>, and the strength will equal <span class="tex-span">5</span>. </p><p>It is not allowed to increase the weight of the edge.</p><p>Your task is to get the tree, which is not broken, by reducing the weight of edges of the given tree, and also all edged should have the positive weight, moreover, the total weight of all edges should be as large as possible.</p><p>It is obvious that the strength of edges can not be negative, however it can equal zero if the weight of the subtree equals zero. </p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree. The next <span class="tex-span"><i>n</i> - 1</span> lines contains the description of edges. Each line contains four integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>&nbsp;— vertices which connect the edge (the vertex number <span class="tex-span"><i>x</i></span> is the parent of the vertex number <span class="tex-span"><i>y</i></span>), <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>p</i></span> are the weight and the strength of the edge, accordingly. It is guaranteed that the edges describe the tree with the root in the vertex <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>If it is impossible to get unbroken tree from the given tree, print <span class="tex-font-style-tt">-1</span> in the only line.</p><p>Otherwise, the output data should contain <span class="tex-span"><i>n</i></span> lines:</p><p>In the first line print the number <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices on the tree. </p><p>In the next <span class="tex-span"><i>n</i> - 1</span> lines print the description of edges of the resulting tree. Each line should contain four integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>&nbsp;— vertices, which the edge connects (the vertex number <span class="tex-span"><i>x</i></span> is the parent of the vertex number <span class="tex-span"><i>y</i></span>), <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>p</i></span> are the new weight and the strength of the edge, accordingly. </p><p>Print edges in the same order as they are given in input data: the first two integers of each line should not be changed. </p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree. The next <span class="tex-span"><i>n</i> - 1</span> lines contains the description of edges. Each line contains four integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>&nbsp;— vertices which connect the edge (the vertex number <span class="tex-span"><i>x</i></span> is the parent of the vertex number <span class="tex-span"><i>y</i></span>), <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>p</i></span> are the weight and the strength of the edge, accordingly. It is guaranteed that the edges describe the tree with the root in the vertex <span class="tex-span">1</span>.</p>

## Output

<p>If it is impossible to get unbroken tree from the given tree, print <span class="tex-font-style-tt">-1</span> in the only line.</p><p>Otherwise, the output data should contain <span class="tex-span"><i>n</i></span> lines:</p><p>In the first line print the number <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices on the tree. </p><p>In the next <span class="tex-span"><i>n</i> - 1</span> lines print the description of edges of the resulting tree. Each line should contain four integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>w</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>&nbsp;— vertices, which the edge connects (the vertex number <span class="tex-span"><i>x</i></span> is the parent of the vertex number <span class="tex-span"><i>y</i></span>), <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>p</i></span> are the new weight and the strength of the edge, accordingly. </p><p>Print edges in the same order as they are given in input data: the first two integers of each line should not be changed. </p>





```input1
3
1 3 5 7
3 2 4 3

```




```input2
4
1 3 2 3
3 4 5 1
3 2 3 3

```




```input3
5
1 2 2 4
2 4 1 9
4 5 5 6
4 3 4 8

```




```input4
7
1 2 5 2
2 3 4 3
1 4 3 7
4 5 4 1
4 6 3 2
6 7 1 6

```




```output1
3
1 3 5 7
3 2 4 3

```




```output2
-1
```




```output3
5
1 2 2 4
2 4 1 9
4 5 1 2
4 3 2 6

```




```output4
7
1 2 5 2
2 3 2 1
1 4 3 7
4 5 3 0
4 6 3 2
6 7 1 6

```


