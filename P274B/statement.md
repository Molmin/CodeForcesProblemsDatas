## Description

<div><p>A <span class="tex-font-style-it">tree</span> is a graph with <span class="tex-span"><i>n</i></span> vertices and exactly <span class="tex-span"><i>n</i> - 1</span> edges; this graph should meet the following condition: there exists exactly one shortest (by number of edges) path between any pair of its vertices.</p><p>A <span class="tex-font-style-it">subtree</span> of a tree <span class="tex-span"><i>T</i></span> is a tree with both vertices and edges as subsets of vertices and edges of <span class="tex-span"><i>T</i></span>.</p><p>You're given a tree with <span class="tex-span"><i>n</i></span> vertices. Consider its vertices numbered with integers from 1 to <span class="tex-span"><i>n</i></span>. Additionally an integer is written on every vertex of this tree. Initially the integer written on the <span class="tex-span"><i>i</i></span>-th vertex is equal to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. In one move you can apply the following operation:</p><ol> <li> Select the subtree of the given tree that includes the vertex with number 1. </li><li> Increase (or decrease) by one all the integers which are written on the vertices of that subtree. </li></ol><p>Calculate the minimum number of moves that is required to make all the integers written on the vertices of the given tree equal to zero.</p></div><div class="input-specification"><p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) indicating there's an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that the input graph is a tree. </p><p>The last line of the input contains a list of <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>v</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the minimum number of operations needed to solve the task.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) indicating there's an edge between vertices <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that the input graph is a tree. </p><p>The last line of the input contains a list of <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>v</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the minimum number of operations needed to solve the task.</p><p>Please, do not write the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
3
1 2
1 3
1 -1 1

```




```output1
3

```


