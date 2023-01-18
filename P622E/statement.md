## Description

<div><p>Tree is a connected graph without cycles. A leaf of a tree is any vertex connected with exactly one other vertex.</p><p>You are given a tree with <span class="tex-span"><i>n</i></span> vertices and a root in the vertex <span class="tex-span">1</span>. There is an ant in each leaf of the tree. In one second some ants can simultaneously go to the parent vertex from the vertex they were in. No two ants can be in the same vertex simultaneously except for the root of the tree.</p><p>Find the minimal time required for all ants to be in the root of the tree. Note that at start the ants are only in the leaves of the tree.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the ends of the <span class="tex-span"><i>i</i></span>-th edge. It is guaranteed that you are given the correct undirected tree.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>t</i></span> — the minimal time required for all ants to be in the root of the tree.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — the number of vertices in the tree.</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the ends of the <span class="tex-span"><i>i</i></span>-th edge. It is guaranteed that you are given the correct undirected tree.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>t</i></span> — the minimal time required for all ants to be in the root of the tree.</p>





```input1
12
1 2
1 3
1 4
2 5
2 6
3 7
3 8
3 9
8 10
8 11
8 12

```




```input2
2
2 1

```




```output1
6

```




```output2
1

```


