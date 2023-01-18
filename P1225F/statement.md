## Description

<div><p>Bytelandian Tree Factory produces trees for all kinds of industrial applications. You have been tasked with optimizing the production of a certain type of tree for an especially large and important order.</p><p>The tree in question is a rooted tree with $n$ vertices labelled with distinct integers from $0$ to $n - 1$. The vertex labelled $0$ is the root of the tree, and for any non-root vertex $v$ the label of its parent $p(v)$ is less than the label of $v$.</p><p>All trees at the factory are made from bamboo blanks. A <span class="tex-font-style-it">bamboo</span> is a rooted tree such that each vertex has exactly one child, except for a single leaf vertex with no children. The vertices of a bamboo blank can be labelled arbitrarily before its processing is started.</p><p>To process a bamboo into another tree a single type of operation can be made: choose an arbitrary non-root vertex $v$ such that its parent $p(v)$ is not a root either. The operation consists of changing the parent of $v$ to its parent's parent $p(p(v))$. Note that parents of all other vertices remain unchanged, in particular, the subtree of $v$ does not change.</p><p>Efficiency is crucial, hence you have to minimize the number of operations to make the desired tree from a bamboo blank. Construct any optimal sequence of operations to produce the desired tree.</p><p>Note that the labelling of the resulting tree has to coincide with the labelling of the desired tree. Formally, the labels of the roots have to be equal, and for non-root vertices with the same label the labels of their parents should be the same.</p><p>It is guaranteed that for any test present in this problem an answer exists, and further, an optimal sequence contains at most $10^6$ operations. Note that <span class="tex-font-style-bf">any hack that does not meet these conditions will be invalid</span>.</p></div><div class="input-specification"><p>The first line contains a single integer $n$&nbsp;— the number of vertices in the tree ($2 \leq n \leq 10^5$).</p><p>The second line contains $n - 1$ integers $p(1), \ldots, p(n - 1)$&nbsp;— indices of parent vertices of $1, \ldots, n - 1$ respectively ($0 \leq p(i) &lt; i$).</p></div><div class="output-specification"><p>In the first line, print $n$ distinct integers $id_1, \ldots, id_n$&nbsp;— the initial labelling of the bamboo blank starting from the root vertex ($0 \leq id_i &lt; n$).</p><p>In the second line, print a single integer $k$&nbsp;— the number of operations in your sequence ($0 \leq k \leq 10^6$).</p><p>In the third line print $k$ integers $v_1, \ldots, v_k$ describing operations in order. The $i$-th operation consists of changing $p(v_i)$ to $p(p(v_i))$. Each operation should be valid, i.e. neither $v_i$ nor $p(v_i)$ can be the root of the tree at the moment.</p></div>

## Input

<p>The first line contains a single integer $n$&nbsp;— the number of vertices in the tree ($2 \leq n \leq 10^5$).</p><p>The second line contains $n - 1$ integers $p(1), \ldots, p(n - 1)$&nbsp;— indices of parent vertices of $1, \ldots, n - 1$ respectively ($0 \leq p(i) &lt; i$).</p>

## Output

<p>In the first line, print $n$ distinct integers $id_1, \ldots, id_n$&nbsp;— the initial labelling of the bamboo blank starting from the root vertex ($0 \leq id_i &lt; n$).</p><p>In the second line, print a single integer $k$&nbsp;— the number of operations in your sequence ($0 \leq k \leq 10^6$).</p><p>In the third line print $k$ integers $v_1, \ldots, v_k$ describing operations in order. The $i$-th operation consists of changing $p(v_i)$ to $p(p(v_i))$. Each operation should be valid, i.e. neither $v_i$ nor $p(v_i)$ can be the root of the tree at the moment.</p>





```input1
5
0 0 1 1
```




```input2
4
0 1 2
```




```output1
0 2 1 4 3
2
1 3
```




```output2
0 1 2 3
0
```


