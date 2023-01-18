## Description

<div><p>A maze is represented by a tree (an undirected graph, where exactly one way exists between each pair of vertices). In the maze the entrance vertex and the exit vertex are chosen with some probability. The exit from the maze is sought by Deep First Search. If there are several possible ways to move, the move is chosen equiprobably. Consider the following pseudo-code:</p><pre class="verbatim"><br>DFS(x)<br>    if x == exit vertex then<br>        <span class="tex-font-style-underline">finish search</span><br>    flag[x] &lt;- TRUE<br>    random shuffle the vertices' order in V(x) // here all permutations have equal probability to be chosen<br>    for i &lt;- 1 to length[V] do<br>        if flag[V[i]] = FALSE then<br>            count++;<br>            DFS(y);<br>    count++;<br></pre><p><span class="tex-span"><i>V</i>(<i>x</i>)</span> is the list vertices adjacent to <span class="tex-span"><i>x</i></span>. The <span class="tex-span"><i>flag</i></span> array is initially filled as <span class="tex-font-style-tt">FALSE</span>. <span class="tex-span"><i>DFS</i></span> initially starts with a parameter of an entrance vertex. When the <span class="tex-font-style-underline">search is finished</span>, variable <span class="tex-span"><i>count</i></span> will contain the number of moves.</p><p>Your task is to count the mathematical expectation of the number of moves one has to do to exit the maze.</p></div><div class="input-specification"><p>The first line determines the number of vertices in the graph <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>n</i> - 1</span> lines contain pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, which show the existence of an edge between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> vertices (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It is guaranteed that the given graph is a tree.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of non-negative numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, which represent the probability of choosing the <span class="tex-span"><i>i</i></span>-th vertex as an entrance and exit correspondingly. The probabilities to choose vertex <span class="tex-span"><i>i</i></span> as an entrance and an exit equal <img align="middle" class="tex-formula" src="file://MxeR68hV.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://oZSAGisv.png" style="max-width: 100.0%;max-height: 100.0%;"> correspondingly. The sum of all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and the sum of all <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are positive and do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print the expectation of the number of moves. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line determines the number of vertices in the graph <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>n</i> - 1</span> lines contain pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, which show the existence of an edge between <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> vertices (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). It is guaranteed that the given graph is a tree.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain pairs of non-negative numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, which represent the probability of choosing the <span class="tex-span"><i>i</i></span>-th vertex as an entrance and exit correspondingly. The probabilities to choose vertex <span class="tex-span"><i>i</i></span> as an entrance and an exit equal <img align="middle" class="tex-formula" src="file://MxeR68hV.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://oZSAGisv.png" style="max-width: 100.0%;max-height: 100.0%;"> correspondingly. The sum of all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and the sum of all <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are positive and do not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print the expectation of the number of moves. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
2
1 2
0 1
1 0

```




```input2
3
1 2
1 3
1 0
0 2
0 3

```




```input3
7
1 2
1 3
2 4
2 5
3 6
3 7
1 1
1 1
1 1
1 1
1 1
1 1
1 1

```




```output1
1.00000000000000000000

```




```output2
2.00000000000000000000

```




```output3
4.04081632653
```



## Note

<p>In the first sample the entrance vertex is always 1 and the exit vertex is always 2.</p><p>In the second sample the entrance vertex is always 1 and the exit vertex with the probability of 2/5 will be 2 of with the probability if 3/5 will be 3. The mathematical expectations for the exit vertices 2 and 3 will be equal (symmetrical cases). During the first move one can go to the exit vertex with the probability of 0.5 or to go to a vertex that's not the exit vertex with the probability of 0.5. In the first case the number of moves equals 1, in the second one it equals 3. The total mathematical expectation is counted as <span class="tex-span">2 / 5 × (1 × 0.5 + 3 × 0.5) + 3 / 5 × (1 × 0.5 + 3 × 0.5)</span></p>
