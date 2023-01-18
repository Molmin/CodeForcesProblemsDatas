## Description

<div><p>Boy Dima gave Julian a birthday present&nbsp;— set $B$ consisting of positive integers. However, he didn't know, that Julian hates sets, but enjoys bipartite graphs more than anything else!</p><p>Julian was almost upset, but her friend Alex said, that he can build an undirected graph using this set in such a way: let all integer numbers be vertices, then connect any two $i$ and $j$ with an edge if $|i - j|$ belongs to $B$.</p><p>Unfortunately, Julian doesn't like the graph, that was built using $B$. Alex decided to rectify the situation, so he wants to erase some numbers from $B$, so that graph built using the new set is bipartite. The difficulty of this task is that the graph, Alex has to work with, has an infinite number of vertices and edges! It is impossible to solve this task alone, so Alex asks you for help. Write a program that erases a subset of <span class="tex-font-style-bf">minimum</span> size from $B$ so that graph constructed on the new set is bipartite.</p><p>Recall, that graph is bipartite if all its vertices can be divided into two disjoint sets such that every edge connects a vertex from different sets.</p></div><div class="input-specification"><p>First line contains an integer $n ~ (1 \leqslant n \leqslant 200\,000)$&nbsp;— size of $B$</p><p>Second line contains $n$ integers $b_1, b_2, \ldots, b_n ~ (1 \leqslant b_i \leqslant 10^{18})$&nbsp;— numbers of $B$, all $b_i$ are <span class="tex-font-style-bf">unique</span></p></div><div class="output-specification"><p>In the first line print single integer $k$ – the number of erased elements. In the second line print $k$ integers&nbsp;— values of erased elements.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>First line contains an integer $n ~ (1 \leqslant n \leqslant 200\,000)$&nbsp;— size of $B$</p><p>Second line contains $n$ integers $b_1, b_2, \ldots, b_n ~ (1 \leqslant b_i \leqslant 10^{18})$&nbsp;— numbers of $B$, all $b_i$ are <span class="tex-font-style-bf">unique</span></p>

## Output

<p>In the first line print single integer $k$ – the number of erased elements. In the second line print $k$ integers&nbsp;— values of erased elements.</p><p>If there are multiple answers, print any of them.</p>





```input1
3
1 2 3
```




```input2
2
2 6
```




```output1
1
2
```




```output2
0
```


