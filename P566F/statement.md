## Description

<div><p>As you must know, the maximum clique problem in an arbitrary graph is <span class="tex-span"><i>NP</i></span>-hard. Nevertheless, for some graphs of specific kinds it can be solved effectively.</p><p>Just in case, let us remind you that a clique in a non-directed graph is a subset of the vertices of a graph, such that any two vertices of this subset are connected by an edge. In particular, an empty set of vertexes and a set consisting of a single vertex, are cliques.</p><p>Let's define a divisibility graph for a set of positive integers <span class="tex-span"><i>A</i> = {<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span> as follows. The vertices of the given graph are numbers from set <span class="tex-span"><i>A</i></span>, and two numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span"><i>i</i> ≠ <i>j</i></span>) are connected by an edge if and only if either <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is divisible by <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, or <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is divisible by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>You are given a set of non-negative integers <span class="tex-span"><i>A</i></span>. Determine the size of a maximum clique in a divisibility graph for set <span class="tex-span"><i>A</i></span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>), that sets the size of set <span class="tex-span"><i>A</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — elements of subset <span class="tex-span"><i>A</i></span>. The numbers in the line follow in the ascending order.</p></div><div class="output-specification"><p>Print a single number — the maximum size of a clique in a divisibility graph for set <span class="tex-span"><i>A</i></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>), that sets the size of set <span class="tex-span"><i>A</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — elements of subset <span class="tex-span"><i>A</i></span>. The numbers in the line follow in the ascending order.</p>

## Output

<p>Print a single number — the maximum size of a clique in a divisibility graph for set <span class="tex-span"><i>A</i></span>.</p>





```input1
8
3 4 6 8 10 18 21 24

```




```output1
3

```



## Note

<p>In the first sample test a clique of size 3 is, for example, a subset of vertexes <span class="tex-span">{3, 6, 18}</span>. A clique of a larger size doesn't exist in this graph.</p>
