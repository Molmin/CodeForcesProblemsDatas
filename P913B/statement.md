## Description

<div><p>Consider a rooted tree. A rooted tree has one special vertex called the root. All edges are directed from the root. Vertex <span class="tex-span"><i>u</i></span> is called a <span class="tex-font-style-it">child</span> of vertex <span class="tex-span"><i>v</i></span> and vertex <span class="tex-span"><i>v</i></span> is called a <span class="tex-font-style-it">parent</span> of vertex <span class="tex-span"><i>u</i></span> if there exists a directed edge from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>. A vertex is called a <span class="tex-font-style-it">leaf</span> if it doesn't have children and has a parent.</p><p>Let's call a rooted tree a <span class="tex-font-style-it">spruce</span> if its every non-leaf vertex has at least <span class="tex-span">3</span> leaf children. You are given a rooted tree, check whether it's a spruce.</p><p>The definition of a rooted tree can be found <a href="https://goo.gl/1dqvzz">here</a>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices in the tree (<span class="tex-span">3 ≤ <i>n</i> ≤ 1 000</span>). Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains one integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>)&nbsp;— the index of the parent of the <span class="tex-span"><i>i</i> + 1</span>-th vertex (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>).</p><p>Vertex <span class="tex-span">1</span> is the root. It's guaranteed that the root has at least <span class="tex-span">2</span> children.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if the tree is a spruce and "<span class="tex-font-style-tt">No</span>" otherwise.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of vertices in the tree (<span class="tex-span">3 ≤ <i>n</i> ≤ 1 000</span>). Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains one integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>)&nbsp;— the index of the parent of the <span class="tex-span"><i>i</i> + 1</span>-th vertex (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i></span>).</p><p>Vertex <span class="tex-span">1</span> is the root. It's guaranteed that the root has at least <span class="tex-span">2</span> children.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if the tree is a spruce and "<span class="tex-font-style-tt">No</span>" otherwise.</p>





```input1
4
1
1
1

```




```input2
7
1
1
1
2
2
2

```




```input3
8
1
1
1
1
3
3
3

```




```output1
Yes

```




```output2
No

```




```output3
Yes

```



## Note

<p>The first example:</p><p><img class="tex-graphics" src="file://TKZ7I0UM.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The second example:</p><p><img class="tex-graphics" src="file://smKbrJZs.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>It is not a spruce, because the non-leaf vertex <span class="tex-span">1</span> has only <span class="tex-span">2</span> leaf children.</p><p>The third example:</p><p><img class="tex-graphics" src="file://bkHH4AaZ.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
