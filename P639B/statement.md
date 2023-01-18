## Description

<div><p>A tree is a connected undirected graph consisting of <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>n</i>  -  1</span> edges. Vertices are numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>.</p><p>Limak is a little polar bear and Radewoosh is his evil enemy. Limak once had a tree but Radewoosh stolen it. Bear is very sad now because he doesn't remember much about the tree&nbsp;— he can tell you only three values <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>h</i></span>:</p><ul> <li> The tree had exactly <span class="tex-span"><i>n</i></span> vertices. </li><li> The tree had diameter <span class="tex-span"><i>d</i></span>. In other words, <span class="tex-span"><i>d</i></span> was the biggest distance between two vertices. </li><li> Limak also remembers that he once rooted the tree in vertex <span class="tex-span">1</span> and after that its height was <span class="tex-span"><i>h</i></span>. In other words, <span class="tex-span"><i>h</i></span> was the biggest distance between vertex <span class="tex-span">1</span> and some other vertex. </li></ul><p>The distance between two vertices of the tree is the number of edges on the simple path between them.</p><p>Help Limak to restore his tree. Check whether there exists a tree satisfying the given conditions. Find any such tree and print its edges in any order. It's also possible that Limak made a mistake and there is no suitable tree&nbsp;– in this case print "<span class="tex-font-style-tt">-1</span>".</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>h</i> ≤ <i>d</i> ≤ <i>n</i> - 1</span>)&nbsp;— the number of vertices, diameter, and height after rooting in vertex <span class="tex-span">1</span>, respectively.</p></div><div class="output-specification"><p>If there is no tree matching what Limak remembers, print the only line with "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>Otherwise, describe any tree matching Limak's description. Print <span class="tex-span"><i>n</i> - 1</span> lines, each with two space-separated integers&nbsp;– indices of vertices connected by an edge. If there are many valid trees, print any of them. You can print edges in any order.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>h</i> ≤ <i>d</i> ≤ <i>n</i> - 1</span>)&nbsp;— the number of vertices, diameter, and height after rooting in vertex <span class="tex-span">1</span>, respectively.</p>

## Output

<p>If there is no tree matching what Limak remembers, print the only line with "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>Otherwise, describe any tree matching Limak's description. Print <span class="tex-span"><i>n</i> - 1</span> lines, each with two space-separated integers&nbsp;– indices of vertices connected by an edge. If there are many valid trees, print any of them. You can print edges in any order.</p>





```input1
5 3 2

```




```input2
8 5 2

```




```input3
8 4 2

```




```output1
1 2
1 3
3 4
3 5
```




```output2
-1

```




```output3
4 8
5 7
2 3
8 1
2 1
5 6
1 5

```



## Note

<p>Below you can see trees printed to the output in the first sample and the third sample.</p><center> <img class="tex-graphics" src="file://FU3KOh4G.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
