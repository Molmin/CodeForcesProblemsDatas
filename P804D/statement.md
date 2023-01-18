## Description

<div><p>Pasha is a good student and one of MoJaK's best friends. He always have a problem to think about. Today they had a talk about the following problem.</p><p>We have a forest (acyclic undirected graph) with <span class="tex-span"><i>n</i></span> vertices and <span class="tex-span"><i>m</i></span> edges. There are <span class="tex-span"><i>q</i></span> queries we should answer. In each query two vertices <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> are given. Let <span class="tex-span"><i>V</i></span> be the set of vertices in the connected component of the graph that contains <span class="tex-span"><i>v</i></span>, and <span class="tex-span"><i>U</i></span> be the set of vertices in the connected component of the graph that contains <span class="tex-span"><i>u</i></span>. Let's add an edge between some vertex <img align="middle" class="tex-formula" src="file://Y2aPMXjl.png" style="max-width: 100.0%;max-height: 100.0%;"> and some vertex in <img align="middle" class="tex-formula" src="file://NwPTS4t2.png" style="max-width: 100.0%;max-height: 100.0%;"> and compute the value <span class="tex-span"><i>d</i></span> of the resulting component. If the resulting component is a tree, the value <span class="tex-span"><i>d</i></span> is the <span class="tex-font-style-it">diameter</span> of the component, and it is equal to <span class="tex-font-style-tt">-1</span> otherwise. What is the expected value of <span class="tex-span"><i>d</i></span>, if we choose vertices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> from the sets uniformly at random?</p><p>Can you help Pasha to solve this problem?</p><p>The <span class="tex-font-style-it">diameter</span> of the component is the maximum <span class="tex-font-style-it">distance</span> among some pair of vertices in the component. The <span class="tex-font-style-it">distance</span> between two vertices is the minimum number of edges on some path between the two vertices.</p><p>Note that queries don't add edges to the initial forest. </p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span>(<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices, the number of edges in the graph and the number of queries.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), that means there is an edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the given graph is a forest.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the vertices given in the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>For each query print the expected value of <span class="tex-span"><i>d</i></span> as described in the problem statement.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the jury's answer is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://45Yrf3qC.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span>(<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of vertices, the number of edges in the graph and the number of queries.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), that means there is an edge between vertices <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It is guaranteed that the given graph is a forest.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the vertices given in the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>For each query print the expected value of <span class="tex-span"><i>d</i></span> as described in the problem statement.</p><p>Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the jury's answer is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://45Yrf3qC.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 1 2
1 3
3 1
2 3

```




```input2
5 2 3
2 4
4 3
4 2
4 1
2 5

```




```output1
-1
2.0000000000

```




```output2
-1
2.6666666667
2.6666666667

```



## Note

<p>In the first example the vertices <span class="tex-span">1</span> and <span class="tex-span">3</span> are in the same component, so the answer for the first query is <span class="tex-font-style-tt">-1</span>. For the second query there are two options to add the edge: one option is to add the edge <span class="tex-span">1 - 2</span>, the other one is <span class="tex-span">2 - 3</span>. In both ways the resulting diameter is <span class="tex-span">2</span>, so the answer is <span class="tex-span">2</span>.</p><p>In the second example the answer for the first query is obviously <span class="tex-font-style-tt">-1</span>. The answer for the second query is the average of three cases: for added edges <span class="tex-span">1 - 2</span> or <span class="tex-span">1 - 3</span> the diameter is <span class="tex-span">3</span>, and for added edge <span class="tex-span">1 - 4</span> the diameter is <span class="tex-span">2</span>. Thus, the answer is <img align="middle" class="tex-formula" src="file://0YSpVIJ1.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
