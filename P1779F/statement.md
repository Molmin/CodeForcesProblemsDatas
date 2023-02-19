## Description

<div><p><span class="tex-font-style-it">Misha had been banned from playing chess for good since he was accused of cheating with an engine. Therefore, he retired and decided to become a xorcerer.</span></p><p>One day, while taking a walk in a park, Misha came across a rooted tree with nodes numbered from $1$ to $n$. The root of the tree is node $1$. </p><p>For each $1\le i\le n$, node $i$ contains $a_i$ stones in it. Misha has recently learned a new spell in his <span class="tex-font-style-it">xorcery</span> class and wants to test it out. A spell consists of:</p><ul> <li> Choose some node $i$ ($1 \leq i \leq n$). </li><li> Calculate the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> $x$ of all $a_j$ such that node $j$ is in the subtree of $i$ ($i$ belongs to its own subtree). </li><li> Set $a_j$ equal to $x$ for all nodes $j$ in the subtree of $i$. </li></ul><p>Misha can perform at most $2n$ spells and he wants to remove all stones from the tree. More formally, he wants $a_i=0$ to hold for each $1\leq i \leq n$. Can you help him perform the spells?</p><p>A tree with $n$ nodes is a connected acyclic graph which contains $n-1$ edges. The subtree of node $i$ is the set of all nodes $j$ such that $i$ lies on the simple path from $1$ (the root) to $j$. We consider $i$ to be contained in its own subtree.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 2\cdot 10^5$)&nbsp;— the size of the tree</p><p>The second line contains an array of integers $a_1,a_2,\ldots, a_n$ ($0 \leq a_i \leq 31$), describing the number of stones in each node initially.</p><p>The third line contains an array of integers $p_2,p_3,\ldots, p_n$ ($1 \leq p_i \leq i-1$), where $p_i$ means that there is an edge connecting $p_i$ and $i$.</p></div><div class="output-specification"><p>If there is not a valid sequence of spells, output $-1$.</p><p>Otherwise, output a single integer $q$ ($0 \leq q \leq 2n$) in the first line&nbsp;— the number of performed spells.</p><p>In the second line output a sequence of integers $v_1,v_2,\ldots,v_q$ ($1 \leq v_i \leq n$)&nbsp;— the $i$-th spell will be performed on the subtree of node $v_i$. Please note that order matters.</p><p>If multiple solutions exist, output any. You don't have to minimize the number of operations.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 2\cdot 10^5$)&nbsp;— the size of the tree</p><p>The second line contains an array of integers $a_1,a_2,\ldots, a_n$ ($0 \leq a_i \leq 31$), describing the number of stones in each node initially.</p><p>The third line contains an array of integers $p_2,p_3,\ldots, p_n$ ($1 \leq p_i \leq i-1$), where $p_i$ means that there is an edge connecting $p_i$ and $i$.</p>

## Output

<p>If there is not a valid sequence of spells, output $-1$.</p><p>Otherwise, output a single integer $q$ ($0 \leq q \leq 2n$) in the first line&nbsp;— the number of performed spells.</p><p>In the second line output a sequence of integers $v_1,v_2,\ldots,v_q$ ($1 \leq v_i \leq n$)&nbsp;— the $i$-th spell will be performed on the subtree of node $v_i$. Please note that order matters.</p><p>If multiple solutions exist, output any. You don't have to minimize the number of operations.</p>





```input1
2
13 13
1
```




```input2
7
5 2 8 3 4 1 31
1 1 2 2 3 3
```




```input3
9
3 31 1 2 7 30 7 3 1
1 1 1 2 5 5 3 4
```




```output1
1
1
```




```output2
-1
```




```output3
6
3 2 3 1 2 2
```



## Note

<p>Please refer to the following pictures for an explanation of the third test. Only the first $4$ spells are shown since the last $2$ do nothing. The first picture represents the tree initially with the number of stones for each node written above it in green. Changes applied by the current spell are highlighted in red.</p><center> <img class="tex-graphics" src="file://940V86qh.png" style="max-width: 100.0%;max-height: 100.0%;">   </center>
