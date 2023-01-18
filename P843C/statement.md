## Description

<div><p>You are given a tree with <span class="tex-span"><i>n</i></span> vertices and you are allowed to perform <span class="tex-font-style-bf">no more than</span> <span class="tex-span">2<i>n</i></span> transformations on it. Transformation is defined by three vertices <span class="tex-span"><i>x</i>, <i>y</i>, <i>y</i>'</span> and consists of deleting edge <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and adding edge <span class="tex-span">(<i>x</i>, <i>y</i>')</span>. Transformation <span class="tex-span"><i>x</i>, <i>y</i>, <i>y</i>'</span> could be performed if all the following conditions are satisfied:</p><ol> <li> There is an edge <span class="tex-span">(<i>x</i>, <i>y</i>)</span> in the current tree. </li><li> After the transformation the graph remains a tree. </li><li> After the deletion of edge <span class="tex-span">(<i>x</i>, <i>y</i>)</span> the tree would consist of two connected components. Let's denote the set of nodes in the component containing vertex <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>V</i><sub class="lower-index"><i>x</i></sub></span>, and the set of nodes in the component containing vertex <span class="tex-span"><i>y</i></span> by <span class="tex-span"><i>V</i><sub class="lower-index"><i>y</i></sub></span>. Then condition <span class="tex-span">|<i>V</i><sub class="lower-index"><i>x</i></sub>| &gt; |<i>V</i><sub class="lower-index"><i>y</i></sub>|</span> should be satisfied, i.e. the size of the component with <span class="tex-span"><i>x</i></span> should be strictly larger than the size of the component with <span class="tex-span"><i>y</i></span>. </li></ol><p>You should <span class="tex-font-style-bf">minimize</span> the sum of squared distances between all pairs of vertices in a tree, which you could get after no more than <span class="tex-span">2<i>n</i></span> transformations and output any sequence of transformations leading initial tree to such state.</p><p>Note that you don't need to minimize the number of operations. It is necessary to minimize only the sum of the squared distances.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of vertices in tree.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines of input contains integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>) — the descriptions of edges. It is guaranteed that the given edges form a tree.</p></div><div class="output-specification"><p>In the first line output integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2<i>n</i></span>) — the number of transformations from your example, <span class="tex-font-style-bf">minimizing</span> sum of squared distances between all pairs of vertices.</p><p>In each of the next <span class="tex-span"><i>k</i></span> lines output three integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>y</i>'</span> — indices of vertices from the corresponding transformation.</p><p>Transformations with <span class="tex-span"><i>y</i> = <i>y</i>'</span> are allowed (even though they don't change tree) if transformation conditions are satisfied.</p><p>If there are several possible answers, print any of them.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of vertices in tree.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines of input contains integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, <i>a</i> ≠ <i>b</i></span>) — the descriptions of edges. It is guaranteed that the given edges form a tree.</p>

## Output

<p>In the first line output integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 2<i>n</i></span>) — the number of transformations from your example, <span class="tex-font-style-bf">minimizing</span> sum of squared distances between all pairs of vertices.</p><p>In each of the next <span class="tex-span"><i>k</i></span> lines output three integers <span class="tex-span"><i>x</i>, <i>y</i>, <i>y</i>'</span> — indices of vertices from the corresponding transformation.</p><p>Transformations with <span class="tex-span"><i>y</i> = <i>y</i>'</span> are allowed (even though they don't change tree) if transformation conditions are satisfied.</p><p>If there are several possible answers, print any of them.</p>





```input1
3
3 2
1 3

```




```input2
7
1 2
2 3
3 4
4 5
5 6
6 7

```




```output1
0

```




```output2
2
4 3 2
4 5 6
```



## Note

<center><p>This is a picture for the second sample. Added edges are dark, deleted edges are dotted.</p><p><img class="tex-graphics" src="file://oCQsGtmp.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center>
