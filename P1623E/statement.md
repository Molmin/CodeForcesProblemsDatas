## Description

<div><p>A binary tree of $n$ nodes is given. Nodes of the tree are numbered from $1$ to $n$ and the root is the node $1$. Each node can have no child, only one left child, only one right child, or both children. For convenience, let's denote $l_u$ and $r_u$ as the left and the right child of the node $u$ respectively, $l_u = 0$ if $u$ does not have the left child, and $r_u = 0$ if the node $u$ does not have the right child.</p><p>Each node has a string label, initially is a single character $c_u$. Let's define the string representation of the binary tree as the concatenation of the labels of the nodes in the <span class="tex-font-style-it">in-order</span>. Formally, let $f(u)$ be the string representation of the tree rooted at the node $u$. $f(u)$ is defined as follows: $$ f(u) = \begin{cases} \texttt{&lt;empty string&gt;}, &amp; \text{if }u = 0; \\ f(l_u) + c_u + f(r_u) &amp; \text{otherwise}, \end{cases} $$ where $+$ denotes the string concatenation operation.</p><p>This way, the string representation of the tree is $f(1)$.</p><p>For each node, we can <span class="tex-font-style-it">duplicate</span> its label <span class="tex-font-style-bf">at most once</span>, that is, assign $c_u$ with $c_u + c_u$, but only if $u$ is the root of the tree, or if its parent also has its label duplicated.</p><p>You are given the tree and an integer $k$. What is the lexicographically smallest string representation of the tree, if we can duplicate labels of at most $k$ nodes?</p><p>A string $a$ is lexicographically smaller than a string $b$ if and only if one of the following holds: </p><ul> <li> $a$ is a prefix of $b$, but $a \ne b$; </li><li> in the first position where $a$ and $b$ differ, the string $a$ has a letter that appears earlier in the alphabet than the corresponding letter in $b$. </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$).</p><p>The second line contains a string $c$ of $n$ lower-case English letters, where $c_i$ is the initial label of the node $i$ for $1 \le i \le n$. Note that the given string $c$ is <span class="tex-font-style-bf">not</span> the initial string representation of the tree.</p><p>The $i$-th of the next $n$ lines contains two integers $l_i$ and $r_i$ ($0 \le l_i, r_i \le n$). If the node $i$ does not have the left child, $l_i = 0$, and if the node $i$ does not have the right child, $r_i = 0$.</p><p>It is guaranteed that the given input forms a binary tree, rooted at $1$.</p></div><div class="output-specification"><p>Print a single line, containing the lexicographically smallest string representation of the tree if at most $k$ nodes have their labels duplicated.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 2 \cdot 10^5$).</p><p>The second line contains a string $c$ of $n$ lower-case English letters, where $c_i$ is the initial label of the node $i$ for $1 \le i \le n$. Note that the given string $c$ is <span class="tex-font-style-bf">not</span> the initial string representation of the tree.</p><p>The $i$-th of the next $n$ lines contains two integers $l_i$ and $r_i$ ($0 \le l_i, r_i \le n$). If the node $i$ does not have the left child, $l_i = 0$, and if the node $i$ does not have the right child, $r_i = 0$.</p><p>It is guaranteed that the given input forms a binary tree, rooted at $1$.</p>

## Output

<p>Print a single line, containing the lexicographically smallest string representation of the tree if at most $k$ nodes have their labels duplicated.</p>





```input1
4 3
abab
2 3
0 0
0 4
0 0
```




```input2
8 2
kadracyn
2 5
3 4
0 0
0 0
6 8
0 7
0 0
0 0
```




```input3
8 3
kdaracyn
2 5
0 3
0 4
0 0
6 8
0 7
0 0
0 0
```




```output1
baaaab
```




```output2
daarkkcyan
```




```output3
darkcyan
```



## Note

<p>The images below present the tree for the examples. The number in each node is the node number, while the subscripted letter is its label. To the right is the string representation of the tree, with each letter having the same color as the corresponding node.</p><p>Here is the tree for the first example. Here we duplicated the labels of nodes $1$ and $3$. We should not duplicate the label of node $2$ because it would give us the string "<span class="tex-font-style-tt">bbaaab</span>", which is lexicographically greater than "<span class="tex-font-style-tt">baaaab</span>".</p><center> <img class="tex-graphics" src="file://z3HgRdV9.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> </center><p>In the second example, we can duplicate the labels of nodes $1$ and $2$. Note that only duplicating the label of the root will produce a worse result than the initial string.</p><center> <img class="tex-graphics" src="file://Lcw1otfX.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> </center><p>In the third example, we should not duplicate any character at all. Even though we would want to duplicate the label of the node $3$, by duplicating it we must also duplicate the label of the node $2$, which produces a worse result.</p><center> <img class="tex-graphics" src="file://Ft5zyxZ9.png" style="max-width: 100.0%;max-height: 100.0%;" width="756px"> </center><p>There is no way to produce string "<span class="tex-font-style-tt">darkkcyan</span>" from a tree with the initial string representation "<span class="tex-font-style-tt">darkcyan</span>" :(.</p>
