## Description

<div><p>Recall that a binary search tree is a rooted binary tree, whose nodes each store a key and each have at most two distinguished subtrees, left and right. The key in each node must be greater than any key stored in the left subtree, and less than any key stored in the right subtree.</p><p>The depth of a vertex is the number of edges on the simple path from the vertex to the root. In particular, the depth of the root is $0$.</p><p>Let's call a binary search tree <span class="tex-font-style-it">perfectly balanced</span> if there doesn't exist a binary search tree with the same number of vertices that has a strictly smaller sum of depths of its vertices.</p><p>Let's call a binary search tree with integer keys <span class="tex-font-style-it">striped</span> if both of the following conditions are satisfied for every vertex $v$: </p><ul> <li> If $v$ has a <span class="tex-font-style-bf">left</span> subtree whose root is $u$, then the parity of the key of $v$ is <span class="tex-font-style-bf">different</span> from the parity of the key of $u$. </li><li> If $v$ has a <span class="tex-font-style-bf">right</span> subtree whose root is $w$, then the parity of the key of $v$ is the <span class="tex-font-style-bf">same</span> as the parity of the key of $w$. </li></ul><p>You are given a single integer $n$. Find the number of perfectly balanced striped binary search trees with $n$ vertices that have distinct integer keys between $1$ and $n$, inclusive. Output this number modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($1 \le n \le 10^6$), denoting the required number of vertices.</p></div><div class="output-specification"><p>Output the number of perfectly balanced striped binary search trees with $n$ vertices and distinct integer keys between $1$ and $n$, inclusive, modulo $998\,244\,353$.</p></div>

## Input

<p>The only line contains a single integer $n$ ($1 \le n \le 10^6$), denoting the required number of vertices.</p>

## Output

<p>Output the number of perfectly balanced striped binary search trees with $n$ vertices and distinct integer keys between $1$ and $n$, inclusive, modulo $998\,244\,353$.</p>





```input1
4
```




```input2
3
```




```output1
1
```




```output2
0
```



## Note

<p>In the first example, this is the only tree that satisfies the conditions: <img class="tex-graphics" src="file://DHepJvET.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second example, here are various trees that don't satisfy some condition: <img class="tex-graphics" src="file://rbcmSW6o.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
