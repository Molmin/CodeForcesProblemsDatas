## Description

<div><p>A group of <span class="tex-span"><i>n</i></span> cities is connected by a network of roads. There is an undirected road between every pair of cities, so there are <img align="middle" class="tex-formula" src="file://aYtKbf1N.png" style="max-width: 100.0%;max-height: 100.0%;"> roads in total. It takes exactly <span class="tex-span"><i>y</i></span> seconds to traverse <span class="tex-font-style-bf">any</span> single road.</p><p>A <span class="tex-font-style-it">spanning tree</span> is a set of roads containing exactly <span class="tex-span"><i>n</i> - 1</span> roads such that it's possible to travel between any two cities using only these roads.</p><p>Some spanning tree of the initial network was chosen. For every road in this tree the time one needs to traverse this road was changed from <span class="tex-span"><i>y</i></span> to <span class="tex-span"><i>x</i></span> seconds. Note that it's not guaranteed that <span class="tex-span"><i>x</i></span> is smaller than <span class="tex-span"><i>y</i></span>.</p><p>You would like to travel through all the cities using the shortest path possible. Given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and a description of the spanning tree that was chosen, find the cost of the shortest path that starts in any city, ends in any city and visits all cities <span class="tex-font-style-bf">exactly once</span>.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains a description of a road in the spanning tree. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that these roads form a spanning tree.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum number of seconds one needs to spend in order to visit all the cities exactly once.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i> - 1</span> lines contains a description of a road in the spanning tree. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that these roads form a spanning tree.</p>

## Output

<p>Print a single integer&nbsp;— the minimum number of seconds one needs to spend in order to visit all the cities exactly once.</p>





```input1
5 2 3
1 2
1 3
3 4
5 3

```




```input2
5 3 2
1 2
1 3
3 4
5 3

```




```output1
9

```




```output2
8

```



## Note

<p>In the first sample, roads of the spanning tree have cost <span class="tex-span">2</span>, while other roads have cost <span class="tex-span">3</span>. One example of an optimal path is <img align="middle" class="tex-formula" src="file://rfbc5ssx.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample, we have the same spanning tree, but roads in the spanning tree cost 3, while other roads cost 2. One example of an optimal path is <img align="middle" class="tex-formula" src="file://DGWHXqHD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
