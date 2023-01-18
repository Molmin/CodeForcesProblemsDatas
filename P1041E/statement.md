## Description

<div><p>Monocarp has drawn a tree (an undirected connected acyclic graph) and then has given each vertex an index. All indices are distinct numbers from $1$ to $n$. For every edge $e$ of this tree, Monocarp has written two numbers: the maximum indices of the vertices of the two components formed if the edge $e$ (and only this edge) is erased from the tree.</p><p>Monocarp has given you a list of $n - 1$ pairs of numbers. He wants you to provide an example of a tree that will produce the said list if this tree exists. If such tree does not exist, say so.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 1\,000$)&nbsp;— the number of vertices in the tree.</p><p>Each of the next $n-1$ lines contains two integers $a_i$ and $b_i$ each ($1 \le a_i &lt; b_i \le n$)&nbsp;— the maximal indices of vertices in the components formed if the $i$-th edge is removed.</p></div><div class="output-specification"><p>If there is no such tree that can produce the given list of pairs, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line and the edges of the tree in the next $n - 1$ lines. Each of the last $n - 1$ lines should contain two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$)&nbsp;— vertices connected by an edge.</p><p><span class="tex-font-style-bf">Note: The numeration of edges doesn't matter for this task. Your solution will be considered correct if your tree produces the same pairs as given in the input file (possibly reordered). That means that you can print the edges of the tree you reconstructed in any order.</span></p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 1\,000$)&nbsp;— the number of vertices in the tree.</p><p>Each of the next $n-1$ lines contains two integers $a_i$ and $b_i$ each ($1 \le a_i &lt; b_i \le n$)&nbsp;— the maximal indices of vertices in the components formed if the $i$-th edge is removed.</p>

## Output

<p>If there is no such tree that can produce the given list of pairs, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line and the edges of the tree in the next $n - 1$ lines. Each of the last $n - 1$ lines should contain two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$)&nbsp;— vertices connected by an edge.</p><p><span class="tex-font-style-bf">Note: The numeration of edges doesn't matter for this task. Your solution will be considered correct if your tree produces the same pairs as given in the input file (possibly reordered). That means that you can print the edges of the tree you reconstructed in any order.</span></p>





```input1
4
3 4
1 4
3 4

```




```input2
3
1 3
1 3

```




```input3
3
1 2
2 3

```




```output1
YES
1 3
3 2
2 4

```




```output2
NO

```




```output3
NO

```



## Note

<p>Possible tree from the first example. Dotted lines show edges you need to remove to get appropriate pairs. </p><center> <img class="tex-graphics" src="file://JmGNyhS1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
