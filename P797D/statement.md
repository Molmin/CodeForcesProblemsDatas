## Description

<div><p>Let <span class="tex-span"><i>T</i></span> be arbitrary binary tree — tree, every vertex of which has no more than two children. Given tree is rooted, so there exists only one vertex which doesn't have a parent — it's the root of a tree. Every vertex has an integer number written on it. Following algorithm is run on every value from the tree <span class="tex-span"><i>T</i></span>:</p><ol> <li> Set pointer to the root of a tree. </li><li> Return success if the value in the current vertex is equal to the number you are looking for </li><li> Go to the left child of the vertex if the value in the current vertex is greater than the number you are looking for </li><li> Go to the right child of the vertex if the value in the current vertex is less than the number you are looking for </li><li> Return fail if you try to go to the vertex that doesn't exist </li></ol><p>Here is the pseudo-code of the described algorithm: </p><pre class="verbatim"><br>bool find(TreeNode t, int x) {<br>    if (t == null)<br>        return false;<br>    if (t.value == x)<br>        return true;<br>    if (x &lt; t.value)<br>        return find(t.left, x);<br>    else<br>        return find(t.right, x);<br>}<br>find(root, x);<br></pre><p>The described algorithm works correctly if the tree is binary search tree (i.e. for each node the values of left subtree are less than the value in the node, the values of right subtree are greater than the value in the node). But it can return invalid result if tree is not a binary search tree.</p><p>Since the given tree is not necessarily a binary search tree, not all numbers can be found this way. Your task is to calculate, how many times the search will fail being running on every value from the tree.</p><p>If the tree has multiple vertices with the same values on them then you should run algorithm on every one of them separately.</p></div><div class="input-specification"><p>First line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of vertices in the tree.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span">3</span> numbers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span>) — value on current vertex, index of the left child of the vertex and index of the right child of the vertex, respectively. If some child doesn't exist then number <span class="tex-span"> - 1</span> is set instead. Note that different vertices of the tree may contain the same values.</p></div><div class="output-specification"><p>Print number of times when search algorithm will fail.</p></div>

## Input

<p>First line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of vertices in the tree.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span">3</span> numbers <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span>) — value on current vertex, index of the left child of the vertex and index of the right child of the vertex, respectively. If some child doesn't exist then number <span class="tex-span"> - 1</span> is set instead. Note that different vertices of the tree may contain the same values.</p>

## Output

<p>Print number of times when search algorithm will fail.</p>





```input1
3
15 -1 -1
10 1 3
5 -1 -1

```




```input2
8
6 2 3
3 4 5
12 6 7
1 -1 8
4 -1 -1
5 -1 -1
14 -1 -1
2 -1 -1

```




```output1
2

```




```output2
1

```



## Note

<p>In the example the root of the tree in vertex <span class="tex-span">2</span>. Search of numbers <span class="tex-span">5</span> and <span class="tex-span">15</span> will return fail because on the first step algorithm will choose the subtree which doesn't contain numbers you are looking for.</p>
