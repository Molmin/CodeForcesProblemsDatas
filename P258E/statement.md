## Description

<div><p>The Little Elephant loves trees very much, he especially loves root trees.</p><p>He's got a tree consisting of <span class="tex-span"><i>n</i></span> nodes (the nodes are numbered from 1 to <span class="tex-span"><i>n</i></span>), with root at node number <span class="tex-span">1</span>. Each node of the tree contains some list of numbers which initially is empty. </p><p>The Little Elephant wants to apply <span class="tex-span"><i>m</i></span> operations. On the <span class="tex-span"><i>i</i></span>-th operation <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>m</i>)</span> he first adds number <span class="tex-span"><i>i</i></span> to lists of all nodes of a subtree with the root in node number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and then he adds number <span class="tex-span"><i>i</i></span> to lists of all nodes of the subtree with root in node <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>After applying all operations the Little Elephant wants to count for each node <span class="tex-span"><i>i</i></span> number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the number of integers <span class="tex-span"><i>j</i></span> <span class="tex-span">(1 ≤ <i>j</i> ≤ <i>n</i>;&nbsp;<i>j</i> ≠ <i>i</i>)</span>, such that the lists of the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th nodes contain at least one common number.</p><p>Help the Little Elephant, count numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> for him.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the tree nodes and the number of operations. </p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>, that mean that there is an edge between nodes number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, that stand for the indexes of the nodes in the <span class="tex-span"><i>i</i></span>-th operation.</p><p>It is guaranteed that the given graph is an undirected tree.</p></div><div class="output-specification"><p>In a single line print <span class="tex-span"><i>n</i></span> space-separated integers — <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the tree nodes and the number of operations. </p><p>Each of the following <span class="tex-span"><i>n</i> - 1</span> lines contains two space-separated integers, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>)</span>, that mean that there is an edge between nodes number <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, that stand for the indexes of the nodes in the <span class="tex-span"><i>i</i></span>-th operation.</p><p>It is guaranteed that the given graph is an undirected tree.</p>

## Output

<p>In a single line print <span class="tex-span"><i>n</i></span> space-separated integers — <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>.</p>





```input1
5 1
1 2
1 3
3 5
3 4
2 3

```




```input2
11 3
1 2
2 3
2 4
1 5
5 6
5 7
5 8
6 9
8 10
8 11
2 9
3 6
2 8

```




```output1
0 3 3 3 3
```




```output2
0 6 7 6 0 2 0 5 4 5 5
```


