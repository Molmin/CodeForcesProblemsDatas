## Description

<div><p>You are given a tree with <span class="tex-span"><i>n</i></span> nodes (numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>) rooted at node <span class="tex-span">1</span>. Also, each node has two values associated with it. The values for <span class="tex-span"><i>i</i></span>-th node are <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>You can jump from a node to any node in its subtree. The cost of one jump from node <span class="tex-span"><i>x</i></span> to node <span class="tex-span"><i>y</i></span> is the product of <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>y</i></sub></span>. The total cost of a path formed by one or more jumps is sum of costs of individual jumps. For every node, calculate the minimum total cost to reach any leaf from that node. Pay attention, that root can never be leaf, even if it has degree <span class="tex-span">1</span>.</p><p>Note that you cannot jump from a node to itself.</p></div><div class="input-specification"><p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of nodes in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub>( - 10<sup class="upper-index">5</sup>  ≤  <i>a</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">5</sup>)</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>,  <i>b</i><sub class="lower-index">2</sub>,  ...,  <i>b</i><sub class="lower-index"><i>n</i></sub>( - 10<sup class="upper-index">5</sup>  ≤  <i>b</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">5</sup>)</span>.</p><p>Next <span class="tex-span"><i>n</i>  -  1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub> ≤  <i>n</i></span>) describing edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in the tree.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>i</i></span>-th of which denotes the minimum cost of a path from node <span class="tex-span"><i>i</i></span> to reach any leaf.</p></div>

## Input

<p>The first line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of nodes in the tree.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub>( - 10<sup class="upper-index">5</sup>  ≤  <i>a</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">5</sup>)</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>,  <i>b</i><sub class="lower-index">2</sub>,  ...,  <i>b</i><sub class="lower-index"><i>n</i></sub>( - 10<sup class="upper-index">5</sup>  ≤  <i>b</i><sub class="lower-index"><i>i</i></sub>  ≤  10<sup class="upper-index">5</sup>)</span>.</p><p>Next <span class="tex-span"><i>n</i>  -  1</span> lines contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>,  <i>v</i><sub class="lower-index"><i>i</i></sub> ≤  <i>n</i></span>) describing edge between nodes <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> in the tree.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>i</i></span>-th of which denotes the minimum cost of a path from node <span class="tex-span"><i>i</i></span> to reach any leaf.</p>





```input1
3
2 10 -1
7 -7 5
2 3
2 1

```




```input2
4
5 -10 5 7
-8 -80 -3 -10
2 1
2 4
1 3

```




```output1
10 50 0
```




```output2
-300 100 0 0
```



## Note

<p>In the first example, node <span class="tex-span">3</span> is already a leaf, so the cost is <span class="tex-span">0</span>. For node <span class="tex-span">2</span>, jump to node <span class="tex-span">3</span> with cost <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> × <i>b</i><sub class="lower-index">3</sub> = 50</span>. For node <span class="tex-span">1</span>, jump directly to node <span class="tex-span">3</span> with cost <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> × <i>b</i><sub class="lower-index">3</sub> = 10</span>.</p><p>In the second example, node <span class="tex-span">3</span> and node <span class="tex-span">4</span> are leaves, so the cost is <span class="tex-span">0</span>. For node <span class="tex-span">2</span>, jump to node <span class="tex-span">4</span> with cost <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> × <i>b</i><sub class="lower-index">4</sub> = 100</span>. For node <span class="tex-span">1</span>, jump to node <span class="tex-span">2</span> with cost <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> × <i>b</i><sub class="lower-index">2</sub> =  - 400</span> followed by a jump from <span class="tex-span">2</span> to <span class="tex-span">4</span> with cost <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> × <i>b</i><sub class="lower-index">4</sub> = 100</span>.</p>
