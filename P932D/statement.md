## Description

<div><p>You are given a node of the tree with index <span class="tex-span">1</span> and with weight <span class="tex-span">0</span>. Let <span class="tex-span"><i>cnt</i></span> be the number of nodes in the tree at any instant (initially, <span class="tex-span"><i>cnt</i></span> is set to <span class="tex-span">1</span>). Support <span class="tex-span"><i>Q</i></span> queries of following two types:</p><ul> <li> <img align="middle" class="tex-formula" src="file://irXk8TZs.png" style="max-width: 100.0%;max-height: 100.0%;"> Add a new node (index <span class="tex-span"><i>cnt</i> + 1</span>) with weight <span class="tex-span"><i>W</i></span> and add edge between node <span class="tex-span"><i>R</i></span> and this node. </li><li> <img align="middle" class="tex-formula" src="file://hb0n3ag2.png" style="max-width: 100.0%;max-height: 100.0%;"> Output the maximum length of sequence of nodes which <ol> <li> starts with <span class="tex-span"><i>R</i></span>. </li><li> Every node in the sequence is an ancestor of its predecessor. </li><li> Sum of weight of nodes in sequence does not exceed <span class="tex-span"><i>X</i></span>. </li><li> For some nodes <span class="tex-span"><i>i</i>, <i>j</i></span> that are consecutive in the sequence if <span class="tex-span"><i>i</i></span> is an ancestor of <span class="tex-span"><i>j</i></span> then <span class="tex-span"><i>w</i>[<i>i</i>] ≥ <i>w</i>[<i>j</i>]</span> and there should not exist a node <span class="tex-span"><i>k</i></span> on simple path from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>w</i>[<i>k</i>] ≥ <i>w</i>[<i>j</i>]</span> </li></ol> </li></ul><p>The tree is rooted at node <span class="tex-span">1</span> at any instant.</p><p><span class="tex-font-style-bf">Note that the queries are given in a modified way.</span></p></div><div class="input-specification"><p>First line containing the number of queries <span class="tex-span"><i>Q</i></span> <span class="tex-span">(1 ≤ <i>Q</i> ≤ 400000)</span>.</p><p>Let <span class="tex-span"><i>last</i></span> be the answer for previous query of type <span class="tex-span">2</span> (initially <span class="tex-span"><i>last</i></span> equals <span class="tex-span">0</span>).</p><p>Each of the next <span class="tex-span"><i>Q</i></span> lines contains a query of following form: </p><ul> <li> 1 p q (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ 10<sup class="upper-index">18</sup></span>): This is query of first type where <img align="middle" class="tex-formula" src="file://MmVOFXdt.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://R5frnoWU.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that <span class="tex-span">1 ≤ <i>R</i> ≤ <i>cnt</i></span> and <span class="tex-span">0 ≤ <i>W</i> ≤ 10<sup class="upper-index">9</sup></span>. </li><li> 2 p q (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ 10<sup class="upper-index">18</sup></span>): This is query of second type where <img align="middle" class="tex-formula" src="file://LGc3bIuW.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://sTJLPvxK.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that <span class="tex-span">1 ≤ <i>R</i> ≤ <i>cnt</i></span> and <span class="tex-span">0 ≤ <i>X</i> ≤ 10<sup class="upper-index">15</sup></span>. </li></ul><p><img align="middle" class="tex-formula" src="file://6GOeHtl0.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes bitwise XOR of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>It is guaranteed that at least one query of type 2 exists.</p></div><div class="output-specification"><p>Output the answer to each query of second type in separate line.</p></div>

## Input

<p>First line containing the number of queries <span class="tex-span"><i>Q</i></span> <span class="tex-span">(1 ≤ <i>Q</i> ≤ 400000)</span>.</p><p>Let <span class="tex-span"><i>last</i></span> be the answer for previous query of type <span class="tex-span">2</span> (initially <span class="tex-span"><i>last</i></span> equals <span class="tex-span">0</span>).</p><p>Each of the next <span class="tex-span"><i>Q</i></span> lines contains a query of following form: </p><ul> <li> 1 p q (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ 10<sup class="upper-index">18</sup></span>): This is query of first type where <img align="middle" class="tex-formula" src="file://MmVOFXdt.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://R5frnoWU.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that <span class="tex-span">1 ≤ <i>R</i> ≤ <i>cnt</i></span> and <span class="tex-span">0 ≤ <i>W</i> ≤ 10<sup class="upper-index">9</sup></span>. </li><li> 2 p q (<span class="tex-span">1 ≤ <i>p</i>, <i>q</i> ≤ 10<sup class="upper-index">18</sup></span>): This is query of second type where <img align="middle" class="tex-formula" src="file://LGc3bIuW.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://sTJLPvxK.png" style="max-width: 100.0%;max-height: 100.0%;">. It is guaranteed that <span class="tex-span">1 ≤ <i>R</i> ≤ <i>cnt</i></span> and <span class="tex-span">0 ≤ <i>X</i> ≤ 10<sup class="upper-index">15</sup></span>. </li></ul><p><img align="middle" class="tex-formula" src="file://6GOeHtl0.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes bitwise XOR of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>It is guaranteed that at least one query of type 2 exists.</p>

## Output

<p>Output the answer to each query of second type in separate line.</p>





```input1
6
1 1 1
2 2 0
2 2 1
1 3 0
2 2 0
2 2 2

```




```input2
6
1 1 0
2 2 0
2 0 3
1 0 2
2 1 3
2 1 6

```




```input3
7
1 1 2
1 2 3
2 3 3
1 0 0
1 5 1
2 5 0
2 4 0

```




```input4
7
1 1 3
1 2 3
2 3 4
1 2 0
1 5 3
2 5 5
2 7 22

```




```output1
0
1
1
2

```




```output2
2
2
3
2

```




```output3
1
1
2

```




```output4
1
2
3

```



## Note

<p>In the first example,</p><p> <span class="tex-span"><i>last</i> = 0</span></p><p>- Query 1: 1 1 1, Node <span class="tex-span">2</span> with weight <span class="tex-span">1</span> is added to node <span class="tex-span">1</span>.</p><p>- Query 2: 2 2 0, No sequence of nodes starting at <span class="tex-span">2</span> has weight less than or equal to <span class="tex-span">0</span>. <span class="tex-span"><i>last</i> = 0</span> </p><p>- Query 3: 2 2 1, Answer is <span class="tex-span">1</span> as sequence will be <span class="tex-span">{2}</span>. <span class="tex-span"><i>last</i> = 1</span></p><p>- Query 4: 1 2 1, Node <span class="tex-span">3</span> with weight <span class="tex-span">1</span> is added to node <span class="tex-span">2</span>. </p><p>- Query 5: 2 3 1, Answer is <span class="tex-span">1</span> as sequence will be <span class="tex-span">{3}</span>. Node <span class="tex-span">2</span> cannot be added as sum of weights cannot be greater than <span class="tex-span">1</span>. <span class="tex-span"><i>last</i> = 1</span></p><p>- Query 6: 2 3 3, Answer is <span class="tex-span">2</span> as sequence will be <span class="tex-span">{3, 2}</span>. <span class="tex-span"><i>last</i> = 2</span></p>
