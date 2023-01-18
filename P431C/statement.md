## Description

<div><p>Quite recently a creative student Lesha had a lecture on trees. After the lecture Lesha was inspired and came up with the tree of his own which he called a <span class="tex-span"><i>k</i></span>-tree.</p><p>A <span class="tex-span"><i>k</i></span>-tree is an infinite rooted tree where:</p><ul> <li> each vertex has exactly <span class="tex-span"><i>k</i></span> children; </li><li> each edge has some weight; </li><li> if we look at the edges that goes from some vertex to its children (exactly <span class="tex-span"><i>k</i></span> edges), then their weights will equal <span class="tex-span">1, 2, 3, ..., <i>k</i></span>. </li></ul><p>The picture below shows a part of a 3-tree.</p><p> </p><center><p> <img class="tex-graphics" src="file://Vs3Y7nk8.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p> </p></center>   As soon as Dima, a good friend of Lesha, found out about the tree, he immediately wondered: "How many paths of total weight <span class="tex-span"><i>n</i></span> (the sum of all weights of the edges in the path) are there, starting from the root of a <span class="tex-span"><i>k</i></span>-tree and also containing at least one edge of weight at least <span class="tex-span"><i>d</i></span>?".<p>Help Dima find an answer to his question. As the number of ways can be rather large, print it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p></div><div class="input-specification"><p>A single line contains three space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100;</span> <span class="tex-span">1 ≤ <i>d</i> ≤ <i>k</i></span>).</p></div><div class="output-specification"><p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p></div>

## Input

<p>A single line contains three space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100;</span> <span class="tex-span">1 ≤ <i>d</i> ≤ <i>k</i></span>).</p>

## Output

<p>Print a single integer — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p>





```input1
3 3 2

```




```input2
3 3 3

```




```input3
4 3 2

```




```input4
4 5 2

```




```output1
3

```




```output2
1

```




```output3
6

```




```output4
7

```


