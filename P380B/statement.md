## Description

<div><p>Sereja adores trees. Today he came up with a revolutionary new type of binary root trees.</p><p>His new tree consists of <span class="tex-span"><i>n</i></span> levels, each vertex is indexed by two integers: the number of the level and the number of the vertex on the current level. The tree root is at level <span class="tex-span">1</span>, its index is <span class="tex-span">(1, 1)</span>. Here is a pseudo code of tree construction.</p><pre class="verbatim"><br>//the global data are integer arrays cnt[], left[][], right[][]<br><br>cnt[1] = 1;<br>fill arrays left[][], right[][] with values -1;<br>for(level = 1; level &lt; n; level = level + 1){<br>    cnt[level + 1] = 0;<br>    for(position = 1; position &lt;= cnt[level]; position = position + 1){<br>        if(the value of position is a power of two){ // that is, 1, 2, 4, 8...<br>            left[level][position] = cnt[level + 1] + 1;<br>            right[level][position] = cnt[level + 1] + 2;<br>            cnt[level + 1] = cnt[level + 1] + 2;            <br>        }else{<br>            right[level][position] = cnt[level + 1] + 1;<br>            cnt[level + 1] = cnt[level + 1] + 1;<br>        }<br>    }<br>}<br></pre><p>After the pseudo code is run, cell <span class="tex-font-style-tt">cnt[level]</span> contains the number of vertices on level <span class="tex-span"><i>level</i></span>. Cell <span class="tex-font-style-tt">left[level][position]</span> contains the number of the vertex on the level <span class="tex-span"><i>level</i> + 1</span>, which is the left child of the vertex with index <span class="tex-span">(<i>level</i>, <i>position</i>)</span>, or it contains -1, if the vertex doesn't have a left child. Similarly, cell <span class="tex-font-style-tt">right[level][position]</span> is responsible for the right child. You can see how the tree with <span class="tex-span"><i>n</i> = 4</span> looks like in the notes.</p><p>Serja loves to make things complicated, so he first made a tree and then added an empty set <span class="tex-span"><i>A</i>(<i>level</i>, <i>position</i>)</span> for each vertex. Then Sereja executes <span class="tex-span"><i>m</i></span> operations. Each operation is of one of the two following types:</p><ul> <li> The format of the operation is "<span class="tex-span">1</span> <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span>". For all vertices <span class="tex-span"><i>level</i>, <i>position</i></span> <span class="tex-span">(<i>level</i> = <i>t</i>;&nbsp;<i>l</i> ≤ <i>position</i> ≤ <i>r</i>)</span> add value <span class="tex-span"><i>x</i></span> to set <span class="tex-span"><i>A</i>(<i>level</i>, <i>position</i>)</span>. </li><li> The format of the operation is "<span class="tex-span">2</span> <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>v</i></span>". For vertex <span class="tex-span"><i>level</i>, <i>position</i></span> <span class="tex-span">(<i>level</i> = <i>t</i>, <i>position</i> = <i>v</i>)</span>, find the union of all sets of vertices that are in the subtree of vertex <span class="tex-span">(<i>level</i>, <i>position</i>)</span>. Print the size of the union of these sets. </li></ul><p>Help Sereja execute the operations. In this problem a set contains only distinct values like std::set in C++.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 7000)</span>. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the operations. The operation of the first type is given by five integers: <span class="tex-span">1</span> <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>cnt</i>[<i>t</i>];&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The operation of the second type is given by three integers: <span class="tex-span">2</span> <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>v</i> ≤ <i>cnt</i>[<i>t</i>])</span>.</p></div><div class="output-specification"><p>For each operation of the second type, print the answer on a single line.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 7000)</span>. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the operations. The operation of the first type is given by five integers: <span class="tex-span">1</span> <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>cnt</i>[<i>t</i>];&nbsp;1 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup>)</span>. The operation of the second type is given by three integers: <span class="tex-span">2</span> <span class="tex-span"><i>t</i></span> <span class="tex-span"><i>v</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>v</i> ≤ <i>cnt</i>[<i>t</i>])</span>.</p>

## Output

<p>For each operation of the second type, print the answer on a single line.</p>





```input1
4 5
1 4 4 7 1
1 3 1 2 2
2 1 1
2 4 1
2 3 3

```




```output1
2
0
1

```



## Note

<p>You can find the definitions that are used while working with root trees by this link: http://en.wikipedia.org/wiki/Tree_(graph_theory)</p><p>You can see an example of a constructed tree at <span class="tex-span"><i>n</i> = 4</span> below.</p><center> <img class="tex-graphics" src="file://QrQkzayV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
