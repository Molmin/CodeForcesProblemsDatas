## Description

<div><p>You are given a tree (a connected acyclic undirected graph) of <span class="tex-span"><i>n</i></span> vertices. Vertices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and each vertex is assigned a character from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">t</span>.</p><p>A path in the tree is said to be palindromic if at least one permutation of the labels in the path is a palindrome.</p><p>For each vertex, output the number of palindromic paths passing through it. </p><p><span class="tex-font-style-bf">Note:</span> The path from vertex <span class="tex-span"><i>u</i></span> to vertex <span class="tex-span"><i>v</i></span> is considered to be the same as the path from vertex <span class="tex-span"><i>v</i></span> to vertex <span class="tex-span"><i>u</i></span>, and this path will be counted only once for each of the vertices it passes through.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) &nbsp;— the number of vertices in the tree.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines each contain two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1  ≤  <i>u</i>, <i>v</i>  ≤  <i>n</i>, <i>u</i> ≠ <i>v</i></span>) denoting an edge connecting vertex <span class="tex-span"><i>u</i></span> and vertex <span class="tex-span"><i>v</i></span>. It is guaranteed that the given graph is a tree.</p><p>The next line contains a string consisting of <span class="tex-span"><i>n</i></span> lowercase characters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">t</span> where the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) character is the label of vertex <span class="tex-span"><i>i</i></span> in the tree.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers in a single line, the <span class="tex-span"><i>i</i></span>-th of which is the number of palindromic paths passing through vertex <span class="tex-span"><i>i</i></span> in the tree.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) &nbsp;— the number of vertices in the tree.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines each contain two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1  ≤  <i>u</i>, <i>v</i>  ≤  <i>n</i>, <i>u</i> ≠ <i>v</i></span>) denoting an edge connecting vertex <span class="tex-span"><i>u</i></span> and vertex <span class="tex-span"><i>v</i></span>. It is guaranteed that the given graph is a tree.</p><p>The next line contains a string consisting of <span class="tex-span"><i>n</i></span> lowercase characters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">t</span> where the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) character is the label of vertex <span class="tex-span"><i>i</i></span> in the tree.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers in a single line, the <span class="tex-span"><i>i</i></span>-th of which is the number of palindromic paths passing through vertex <span class="tex-span"><i>i</i></span> in the tree.</p>





```input1
5
1 2
2 3
3 4
3 5
abcbb

```




```input2
7
6 2
4 3
3 7
5 2
7 2
1 4
afefdfs

```




```output1
1 3 4 3 3 

```




```output2
1 4 1 1 2 4 2 

```



## Note

<p>In the first sample case, the following paths are palindromic:</p><p><span class="tex-span">2 - 3 - 4</span></p><p><span class="tex-span">2 - 3 - 5</span></p><p><span class="tex-span">4 - 3 - 5</span></p><p>Additionally, all paths containing only one vertex are palindromic. Listed below are a few paths in the first sample that are not palindromic:</p><p><span class="tex-span">1 - 2 - 3</span></p><p><span class="tex-span">1 - 2 - 3 - 4</span></p><p><span class="tex-span">1 - 2 - 3 - 5</span></p>
