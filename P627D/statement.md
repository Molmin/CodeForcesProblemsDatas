## Description

<div><p>For his computer science class, Jacob builds a model tree with sticks and balls containing <span class="tex-span"><i>n</i></span> nodes in the shape of a tree. Jacob has spent <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> minutes building the <span class="tex-span"><i>i</i></span>-th ball in the tree.</p><p>Jacob's teacher will evaluate his model and grade Jacob based on the effort he has put in. However, she does not have enough time to search his whole tree to determine this; Jacob knows that she will examine the first <span class="tex-span"><i>k</i></span> nodes in a DFS-order traversal of the tree. She will then assign Jacob a grade equal to the minimum <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> she finds among those <span class="tex-span"><i>k</i></span> nodes.</p><p>Though Jacob does not have enough time to rebuild his model, he can choose the root node that his teacher starts from. Furthermore, he can rearrange the list of neighbors of <span class="tex-font-style-bf">each node</span> in any order he likes. Help Jacob find the best grade he can get on this assignment.</p><p>A DFS-order traversal is an ordering of the nodes of a rooted tree, built by a recursive DFS-procedure initially called on the root of the tree. When called on a given node <span class="tex-span"><i>v</i></span>, the procedure does the following: </p><ol> <li> Print <span class="tex-span"><i>v</i></span>. </li><li> Traverse the list of neighbors of the node <span class="tex-span"><i>v</i></span> in order and iteratively call DFS-procedure on each one. Do not call DFS-procedure on node <span class="tex-span"><i>u</i></span> if you came to node <span class="tex-span"><i>v</i></span> directly from <span class="tex-span"><i>u</i></span>. </li></ol></div><div class="input-specification"><p>The first line of the input contains two positive integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of balls in Jacob's tree and the number of balls the teacher will inspect.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>), the time Jacob used to build the <span class="tex-span"><i>i</i></span>-th ball.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>) representing a connection in Jacob's tree between balls <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum grade Jacob can get by picking the right root of the tree and rearranging the list of neighbors.</p></div>

## Input

<p>The first line of the input contains two positive integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of balls in Jacob's tree and the number of balls the teacher will inspect.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>), the time Jacob used to build the <span class="tex-span"><i>i</i></span>-th ball.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>) representing a connection in Jacob's tree between balls <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print a single integer&nbsp;— the maximum grade Jacob can get by picking the right root of the tree and rearranging the list of neighbors.</p>





```input1
5 3
3 6 1 4 2
1 2
2 4
2 5
1 3

```




```input2
4 2
1 5 5 5
1 2
1 3
1 4

```




```output1
3

```




```output2
1

```



## Note

<p>In the first sample, Jacob can root the tree at node <span class="tex-span">2</span> and order <span class="tex-span">2</span>'s neighbors in the order <span class="tex-span">4</span>, <span class="tex-span">1</span>, <span class="tex-span">5</span> (all other nodes have at most two neighbors). The resulting preorder traversal is <span class="tex-span">2</span>, <span class="tex-span">4</span>, <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span>, and the minimum <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of the first <span class="tex-span">3</span> nodes is <span class="tex-span">3</span>.</p><p>In the second sample, it is clear that any preorder traversal will contain node <span class="tex-span">1</span> as either its first or second node, so Jacob cannot do better than a grade of <span class="tex-span">1</span>.</p>
