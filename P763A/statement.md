## Description

<div><p>Each New Year Timofey and his friends cut down a tree of <span class="tex-span"><i>n</i></span> vertices and bring it home. After that they paint all the <span class="tex-span"><i>n</i></span> its vertices, so that the <span class="tex-span"><i>i</i></span>-th vertex gets color <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Now it's time for Timofey birthday, and his mother asked him to remove the tree. Timofey removes the tree in the following way: he takes some vertex in hands, while all the other vertices move down so that the tree becomes rooted at the chosen vertex. After that Timofey brings the tree to a trash can.</p><p>Timofey doesn't like it when many colors are mixing together. A subtree annoys him if there are vertices of different color in it. Timofey wants to find a vertex which he should take in hands so that there are no subtrees that annoy him. He doesn't consider the whole tree as a subtree since he can't see the color of the root vertex.</p><p>A subtree of some vertex is a subgraph containing that vertex and all its descendants.</p><p>Your task is to determine if there is a vertex, taking which in hands Timofey wouldn't be annoyed.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>), denoting there is an edge between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that the given graph is a tree.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), denoting the colors of the vertices.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" in a single line, if Timofey can't take the tree in such a way that it doesn't annoy him.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line print the index of the vertex which Timofey should take in hands. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices in the tree.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i> ≠ <i>v</i></span>), denoting there is an edge between vertices <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>. It is guaranteed that the given graph is a tree.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), denoting the colors of the vertices.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" in a single line, if Timofey can't take the tree in such a way that it doesn't annoy him.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line print the index of the vertex which Timofey should take in hands. If there are multiple answers, print any of them.</p>





```input1
4
1 2
2 3
3 4
1 2 1 1

```




```input2
3
1 2
2 3
1 2 3

```




```input3
4
1 2
2 3
3 4
1 2 1 2

```




```output1
YES
2
```




```output2
YES
2
```




```output3
NO
```


