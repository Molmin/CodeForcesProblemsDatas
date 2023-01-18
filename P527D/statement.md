## Description

<div><p>The clique problem is one of the most well-known NP-complete problems. Under some simplification it can be formulated as follows. Consider an undirected graph <span class="tex-span"><i>G</i></span>. It is required to find a subset of vertices <span class="tex-span"><i>C</i></span> of the maximum size such that any two of them are connected by an edge in graph <span class="tex-span"><i>G</i></span>. Sounds simple, doesn't it? Nobody yet knows an algorithm that finds a solution to this problem in polynomial time of the size of the graph. However, as with many other NP-complete problems, the clique problem is easier if you consider a specific type of a graph.</p><p>Consider <span class="tex-span"><i>n</i></span> distinct points on a line. Let the <span class="tex-span"><i>i</i></span>-th point have the coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. Let's form graph <span class="tex-span"><i>G</i></span>, whose vertices are these points and edges connect exactly the pairs of points <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, such that the distance between them is not less than the sum of their weights, or more formally: <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>j</i></sub>| ≥ <i>w</i><sub class="lower-index"><i>i</i></sub> + <i>w</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Find the size of the maximum clique in such graph.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of points.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinate and the weight of a point. All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are different.</p></div><div class="output-specification"><p>Print a single number — the number of vertexes in the maximum clique of the given graph.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of points.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the coordinate and the weight of a point. All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are different.</p>

## Output

<p>Print a single number — the number of vertexes in the maximum clique of the given graph.</p>





```input1
4
2 3
3 1
6 1
0 2

```




```output1
3

```



## Note

<p>If you happen to know how to solve this problem without using the specific properties of the graph formulated in the problem statement, then you are able to get a prize of one million dollars!</p><p>The picture for the sample test.</p><center> <img class="tex-graphics" src="file://hkhK8GQe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
