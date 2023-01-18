## Description

<div><p>Roman planted a tree consisting of <span class="tex-span"><i>n</i></span> vertices. Each vertex contains a lowercase English letter. Vertex <span class="tex-span">1</span> is the root of the tree, each of the <span class="tex-span"><i>n</i> - 1</span> remaining vertices has a <span class="tex-font-style-it">parent</span> in the tree. Vertex is connected with its parent by an edge. The parent of vertex <span class="tex-span"><i>i</i></span> is vertex <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, the parent index is always less than the index of the vertex (i.e., <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>).</p><p>The <span class="tex-font-style-it">depth</span> of the vertex is the number of nodes on the path from the root to <span class="tex-span"><i>v</i></span> along the edges. In particular, the depth of the root is equal to <span class="tex-span">1</span>.</p><p>We say that vertex <span class="tex-span"><i>u</i></span> is in the <span class="tex-font-style-it">subtree</span> of vertex <span class="tex-span"><i>v</i></span>, if we can get from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span>, moving from the vertex to the parent. In particular, vertex <span class="tex-span"><i>v</i></span> is in its subtree.</p><p>Roma gives you <span class="tex-span"><i>m</i></span> queries, the <span class="tex-span"><i>i</i></span>-th of which consists of two numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Let's consider the vertices in the subtree <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> located at depth <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Determine whether you can use the letters written at these vertices to make a string that is a <span class="tex-font-style-it">palindrome</span>. The letters that are written in the vertexes, can be rearranged in any order to make a palindrome, but all letters should be used.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500 000</span>) — the number of nodes in the tree and queries, respectively.</p><p>The following line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the parents of vertices from the second to the <span class="tex-span"><i>n</i></span>-th (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> lowercase English letters, the <span class="tex-span"><i>i</i></span>-th of these letters is written on vertex <span class="tex-span"><i>i</i></span>.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the queries, the <span class="tex-span"><i>i</i></span>-th line contains two numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the vertex and the depth that appear in the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if in the <span class="tex-span"><i>i</i></span>-th query you can make a palindrome from the letters written on the vertices, otherwise print "<span class="tex-font-style-tt">No</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 500 000</span>) — the number of nodes in the tree and queries, respectively.</p><p>The following line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> — the parents of vertices from the second to the <span class="tex-span"><i>n</i></span>-th (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> lowercase English letters, the <span class="tex-span"><i>i</i></span>-th of these letters is written on vertex <span class="tex-span"><i>i</i></span>.</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the queries, the <span class="tex-span"><i>i</i></span>-th line contains two numbers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the vertex and the depth that appear in the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th line print "<span class="tex-font-style-tt">Yes</span>" (without the quotes), if in the <span class="tex-span"><i>i</i></span>-th query you can make a palindrome from the letters written on the vertices, otherwise print "<span class="tex-font-style-tt">No</span>" (without the quotes).</p>





```input1
6 5
1 1 1 3 3
zacccd
1 1
3 3
4 1
6 1
1 2

```




```output1
Yes
No
Yes
Yes
Yes

```



## Note

<p>String <span class="tex-span"><i>s</i></span> is a <span class="tex-font-style-it">palindrome</span> if reads the same from left to right and from right to left. In particular, an empty string is a palindrome.</p><p>Clarification for the sample test.</p><p>In the first query there exists only a vertex 1 satisfying all the conditions, we can form a palindrome "<span class="tex-font-style-tt">z</span>".</p><p>In the second query vertices 5 and 6 satisfy condititions, they contain letters "<span class="tex-font-style-tt">с</span>" and "<span class="tex-font-style-tt">d</span>" respectively. It is impossible to form a palindrome of them.</p><p>In the third query there exist no vertices at depth 1 and in subtree of 4. We may form an empty palindrome.</p><p>In the fourth query there exist no vertices <span class="tex-font-style-bf">in subtree of 6 at depth 1</span>. We may form an empty palindrome.</p><p>In the fifth query there vertices 2, 3 and 4 satisfying all conditions above, they contain letters "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">c</span>" and "<span class="tex-font-style-tt">c</span>". We may form a palindrome "<span class="tex-font-style-tt">cac</span>".</p>
