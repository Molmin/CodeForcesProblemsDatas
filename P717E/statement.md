## Description

<div><p>I see a pink boar and I want it painted black. Black boars look much more awesome and mighty than the pink ones. Since Jaggy became the ruler of the forest, he has been trying his best to improve the diplomatic relations between the forest region and the nearby ones. </p><p>Some other rulers, however, have requested too much in return for peace between their two regions, so he realized he has to resort to intimidation. Once a delegate for diplomatic relations of a neighboring region visits Jaggy’s forest, if they see a whole bunch of black boars, they might suddenly change their mind about attacking Jaggy. Black boars are really scary, after all. </p><p>Jaggy’s forest can be represented as a tree (connected graph without cycles) with <span class="tex-span"><i>n</i></span> vertices. Each vertex represents a boar and is colored either black or pink. Jaggy has sent a squirrel to travel through the forest and paint all the boars black. The squirrel, however, is quite unusually trained and while it traverses the graph, it changes the color of every vertex it visits, regardless of its initial color: pink vertices become black and black vertices become pink. </p><p>Since Jaggy is too busy to plan the squirrel’s route, he needs your help. He wants you to construct a walk through the tree starting from vertex <span class="tex-span">1</span> such that in the end all vertices are black. A walk is a sequence of vertices, such that every consecutive pair has an edge between them in a tree.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>), denoting the number of vertices in the tree. The following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers, which represent the color of the nodes.</p><p>If the <span class="tex-span"><i>i</i></span>-th integer is <span class="tex-span">1</span>, if the <span class="tex-span"><i>i</i></span>-th vertex is black and <span class="tex-span"> - 1</span> if the <span class="tex-span"><i>i</i></span>-th vertex is pink.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers, which represent the indexes of the vertices which are connected by the edge. Vertices are numbered starting with <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>Output path of a squirrel: output a sequence of visited nodes' indexes in order of visiting. In case of all the nodes are initially black, you should print <span class="tex-span">1</span>. Solution is guaranteed to exist. If there are multiple solutions to the problem you can output any of them provided length of sequence is not longer than <span class="tex-span">10<sup class="upper-index">7</sup></span>.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>), denoting the number of vertices in the tree. The following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>n</i></span> integers, which represent the color of the nodes.</p><p>If the <span class="tex-span"><i>i</i></span>-th integer is <span class="tex-span">1</span>, if the <span class="tex-span"><i>i</i></span>-th vertex is black and <span class="tex-span"> - 1</span> if the <span class="tex-span"><i>i</i></span>-th vertex is pink.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers, which represent the indexes of the vertices which are connected by the edge. Vertices are numbered starting with <span class="tex-span">1</span>.</p>

## Output

<p>Output path of a squirrel: output a sequence of visited nodes' indexes in order of visiting. In case of all the nodes are initially black, you should print <span class="tex-span">1</span>. Solution is guaranteed to exist. If there are multiple solutions to the problem you can output any of them provided length of sequence is not longer than <span class="tex-span">10<sup class="upper-index">7</sup></span>.</p>





```input1
5
1
1
-1
1
-1
2 5
4 3
2 4
4 1

```




```output1
1 4 2 5 2 4 3 4 1 4 1

```



## Note

<p>At the beginning squirrel is at node 1 and its color is black. Next steps are as follows: </p><ul> <li> From node <span class="tex-span">1</span> we walk to node <span class="tex-span">4</span> and change its color to pink. </li><li> From node <span class="tex-span">4</span> we walk to node <span class="tex-span">2</span> and change its color to pink. </li><li> From node <span class="tex-span">2</span> we walk to node <span class="tex-span">5</span> and change its color to black. </li><li> From node <span class="tex-span">5</span> we return to node <span class="tex-span">2</span> and change its color to black. </li><li> From node <span class="tex-span">2</span> we walk to node <span class="tex-span">4</span> and change its color to black. </li><li> We visit node <span class="tex-span">3</span> and change its color to black. </li><li> We visit node <span class="tex-span">4</span> and change its color to pink. </li><li> We visit node <span class="tex-span">1</span> and change its color to pink. </li><li> We visit node <span class="tex-span">4</span> and change its color to black. </li><li> We visit node <span class="tex-span">1</span> and change its color to black. </li></ul>
