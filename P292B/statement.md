## Description

<div><p><span class="tex-font-style-it">This problem uses a simplified network topology model, please read the problem statement carefully and use it as a formal document as you develop the solution.</span></p><p>Polycarpus continues working as a system administrator in a large corporation. The computer network of this corporation consists of <span class="tex-span"><i>n</i></span> computers, some of them are connected by a cable. The computers are indexed by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It's known that any two computers connected by cable directly or through other computers</p><p>Polycarpus decided to find out the network's topology. A network topology is the way of describing the network configuration, the scheme that shows the location and the connections of network devices.</p><p>Polycarpus knows three main network topologies: bus, ring and star. A bus is the topology that represents a shared cable with all computers connected with it. In the ring topology the cable connects each computer only with two other ones. A star is the topology where all computers of a network are connected to the single central node.</p><p>Let's represent each of these network topologies as a connected non-directed graph. A bus is a connected graph that is the only path, that is, the graph where all nodes are connected with two other ones except for some two nodes that are the beginning and the end of the path. A ring is a connected graph, where all nodes are connected with two other ones. A star is a connected graph, where a single central node is singled out and connected with all other nodes. For clarifications, see the picture.</p><center> <img class="tex-graphics" src="file://lgZdwwAc.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-script">(1) — bus, (2) — ring, (3) — star</span> </center><p>You've got a connected non-directed graph that characterizes the computer network in Polycarpus' corporation. Help him find out, which topology type the given network is. If that is impossible to do, say that the network's topology is unknown. </p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(4 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;3 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes and edges in the graph, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain the description of the graph's edges. The <span class="tex-span"><i>i</i></span>-th line contains a space-separated pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of nodes that are connected by the <span class="tex-span"><i>i</i></span>-the edge.</p><p>It is guaranteed that the given graph is connected. There is at most one edge between any two nodes. No edge connects a node with itself.</p></div><div class="output-specification"><p>In a single line print the network topology name of the given graph. If the answer is the bus, print "<span class="tex-font-style-tt">bus topology</span>" (without the quotes), if the answer is the ring, print "<span class="tex-font-style-tt">ring topology</span>" (without the quotes), if the answer is the star, print "<span class="tex-font-style-tt">star topology</span>" (without the quotes). If no answer fits, print "<span class="tex-font-style-tt">unknown topology</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(4 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;3 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of nodes and edges in the graph, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain the description of the graph's edges. The <span class="tex-span"><i>i</i></span>-th line contains a space-separated pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the numbers of nodes that are connected by the <span class="tex-span"><i>i</i></span>-the edge.</p><p>It is guaranteed that the given graph is connected. There is at most one edge between any two nodes. No edge connects a node with itself.</p>

## Output

<p>In a single line print the network topology name of the given graph. If the answer is the bus, print "<span class="tex-font-style-tt">bus topology</span>" (without the quotes), if the answer is the ring, print "<span class="tex-font-style-tt">ring topology</span>" (without the quotes), if the answer is the star, print "<span class="tex-font-style-tt">star topology</span>" (without the quotes). If no answer fits, print "<span class="tex-font-style-tt">unknown topology</span>" (without the quotes).</p>





```input1
4 3
1 2
2 3
3 4

```




```input2
4 4
1 2
2 3
3 4
4 1

```




```input3
4 3
1 2
1 3
1 4

```




```input4
4 4
1 2
2 3
3 1
1 4

```




```output1
bus topology

```




```output2
ring topology

```




```output3
star topology

```




```output4
unknown topology

```


