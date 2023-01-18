## Description

<div><p>Сity N. has a huge problem with roads, food and IT-infrastructure. In total the city has <span class="tex-span"><i>n</i></span> junctions, some pairs of them are connected by bidirectional roads. The road network consists of <span class="tex-span"><i>n</i> - 1</span> roads, you can get from any junction to any other one by these roads. Yes, you're right — the road network forms an undirected tree.</p><p>Recently, the Mayor came up with a way that eliminates the problems with the food and the IT-infrastructure at the same time! He decided to put at the city junctions restaurants of two well-known cafe networks for IT professionals: "iMac D0naldz" and "Burger Bing". Since the network owners are not friends, it is strictly prohibited to place two restaurants of different networks on neighboring junctions. There are other requirements. Here's the full list:</p><ul> <li> each junction must have at most one restaurant; </li><li> each restaurant belongs either to "iMac D0naldz", or to "Burger Bing"; </li><li> each network should build at least one restaurant; </li><li> there is no pair of junctions that are connected by a road and contains restaurants of different networks. </li></ul><p>The Mayor is going to take a large tax from each restaurant, so he is interested in making the total number of the restaurants as large as possible.</p><p>Help the Mayor to analyze the situation. Find all such pairs of <span class="tex-span">(<i>a</i>, <i>b</i>)</span> that <span class="tex-span"><i>a</i></span> restaurants can belong to "iMac D0naldz", <span class="tex-span"><i>b</i></span> restaurants can belong to "Burger Bing", and the sum of <span class="tex-span"><i>a</i> + <i>b</i></span> is as large as possible.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 5000)</span> — the number of junctions in the city. Next <span class="tex-span"><i>n</i> - 1</span> lines list all roads one per line. Each road is given as a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the indexes of connected junctions. Consider the junctions indexed from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that the given road network is represented by an undirected tree with <span class="tex-span"><i>n</i></span> vertexes.</p></div><div class="output-specification"><p>Print on the first line integer <span class="tex-span"><i>z</i></span> — the number of sought pairs. Then print all sought pairs <span class="tex-span">(<i>a</i>, <i>b</i>)</span> in the order of increasing of the first component <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 5000)</span> — the number of junctions in the city. Next <span class="tex-span"><i>n</i> - 1</span> lines list all roads one per line. Each road is given as a pair of integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the indexes of connected junctions. Consider the junctions indexed from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that the given road network is represented by an undirected tree with <span class="tex-span"><i>n</i></span> vertexes.</p>

## Output

<p>Print on the first line integer <span class="tex-span"><i>z</i></span> — the number of sought pairs. Then print all sought pairs <span class="tex-span">(<i>a</i>, <i>b</i>)</span> in the order of increasing of the first component <span class="tex-span"><i>a</i></span>.</p>





```input1
5
1 2
2 3
3 4
4 5

```




```input2
10
1 2
2 3
3 4
5 6
6 7
7 4
8 9
9 10
10 4

```




```output1
3
1 3
2 2
3 1

```




```output2
6
1 8
2 7
3 6
6 3
7 2
8 1

```



## Note

<p>The figure below shows the answers to the first test case. The junctions with "iMac D0naldz" restaurants are marked red and "Burger Bing" restaurants are marked blue.</p><p><img class="tex-graphics" src="file://IHPtQIU1.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
