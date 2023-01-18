## Description

<div><p>You have a full binary tree having infinite levels.</p><p>Each node has an initial value. If a node has value <span class="tex-span"><i>x</i></span>, then its left child has value <span class="tex-span">2·<i>x</i></span> and its right child has value <span class="tex-span">2·<i>x</i> + 1</span>. </p><p>The value of the root is <span class="tex-span">1</span>. </p><p>You need to answer <span class="tex-span"><i>Q</i></span> queries. </p><p>There are <span class="tex-span">3</span> types of queries: </p><ol><li> Cyclically shift the <span class="tex-font-style-bf"><span class="tex-font-style-it">values</span></span> of all nodes on the same level as node with value <span class="tex-span"><i>X</i></span> by <span class="tex-span"><i>K</i></span> units. (The values/nodes of any other level are not affected).</li><li> Cyclically shift the <span class="tex-font-style-bf"><span class="tex-font-style-it">nodes</span></span> on the same level as node with value <span class="tex-span"><i>X</i></span> by <span class="tex-span"><i>K</i></span> units. (The subtrees of these nodes will move along with them).</li><li> Print the value of every node encountered on the simple path from the node with value <span class="tex-span"><i>X</i></span> to the root.</li></ol><p>Positive <span class="tex-span"><i>K</i></span> implies right cyclic shift and negative <span class="tex-span"><i>K</i></span> implies left cyclic shift. </p><p>It is guaranteed that atleast one type <span class="tex-span">3</span> query is present.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Then <span class="tex-span"><i>Q</i></span> queries follow, one per line: </p><ul><li> Queries of type <span class="tex-span">1</span> and <span class="tex-span">2</span> have the following format: <span class="tex-span"><i>T</i></span> <span class="tex-span"><i>X</i></span> <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 2</span>; <span class="tex-span">1 ≤ <i>X</i> ≤ 10<sup class="upper-index">18</sup></span>; <span class="tex-span">0 ≤ |<i>K</i>| ≤ 10<sup class="upper-index">18</sup></span>), where <span class="tex-span"><i>T</i></span> is type of the query.</li><li> Queries of type <span class="tex-span">3</span> have the following format: <span class="tex-span">3</span> <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>X</i> ≤ 10<sup class="upper-index">18</sup></span>).</li></ul></div><div class="output-specification"><p>For each query of type <span class="tex-span">3</span>, print the values of all nodes encountered in descending order.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>Q</i></span> (<span class="tex-span">1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Then <span class="tex-span"><i>Q</i></span> queries follow, one per line: </p><ul><li> Queries of type <span class="tex-span">1</span> and <span class="tex-span">2</span> have the following format: <span class="tex-span"><i>T</i></span> <span class="tex-span"><i>X</i></span> <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 2</span>; <span class="tex-span">1 ≤ <i>X</i> ≤ 10<sup class="upper-index">18</sup></span>; <span class="tex-span">0 ≤ |<i>K</i>| ≤ 10<sup class="upper-index">18</sup></span>), where <span class="tex-span"><i>T</i></span> is type of the query.</li><li> Queries of type <span class="tex-span">3</span> have the following format: <span class="tex-span">3</span> <span class="tex-span"><i>X</i></span> (<span class="tex-span">1 ≤ <i>X</i> ≤ 10<sup class="upper-index">18</sup></span>).</li></ul>

## Output

<p>For each query of type <span class="tex-span">3</span>, print the values of all nodes encountered in descending order.</p>





```input1
5
3 12
1 2 1
3 12
2 4 -1
3 8

```




```input2
5
3 14
1 5 -3
3 14
1 3 1
3 14

```




```output1
12 6 3 1 
12 6 2 1 
8 4 2 1 

```




```output2
14 7 3 1 
14 6 3 1 
14 6 2 1 

```



## Note

<p>Following are the images of the first <span class="tex-span">4</span> levels of the tree in the first test case:</p><p>Original: </p><center> <img class="tex-graphics" src="file://0njcmEJU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p> After query <span class="tex-font-style-it">1 2 1</span>: </p><center> <img class="tex-graphics" src="file://KOFmwCMZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p> After query <span class="tex-font-style-it">2 4 -1</span>: </p><center> <img class="tex-graphics" src="file://vPVd94A2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
