## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities numbered from 1 to <span class="tex-span"><i>n</i></span> in Berland. Some of them are connected by two-way roads. Each road has its own length — an integer number from 1 to 1000. It is known that from each city it is possible to get to any other city by existing roads. Also for each pair of cities it is known the shortest distance between them. Berland Government plans to build <span class="tex-span"><i>k</i></span> new roads. For each of the planned road it is known its length, and what cities it will connect. To control the correctness of the construction of new roads, after the opening of another road Berland government wants to check the sum of the shortest distances between all pairs of cities. Help them — for a given matrix of shortest distances on the old roads and plans of all new roads, find out how the sum of the shortest distances between all pairs of cities changes after construction of each road.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 300</span>) — amount of cities in Berland. Then there follow <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> integer numbers each — the matrix of shortest distances. <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th row — <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>, the shortest distance between cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. It is guaranteed that <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0, <i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>d</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span>, and a given matrix is a matrix of shortest distances for some set of two-way roads with integer lengths from 1 to 1000, such that from each city it is possible to get to any other city using these roads.</p><p>Next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 300</span>) — amount of planned roads. Following <span class="tex-span"><i>k</i></span> lines contain the description of the planned roads. Each road is described by three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — pair of cities, which the road connects, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the length of the road. It can be several roads between a pair of cities, but no road connects the city with itself.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>). <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> should be equal to the sum of shortest distances between all pairs of cities after the construction of roads with indexes from 1 to <span class="tex-span"><i>i</i></span>. Roads are numbered from 1 in the input order. Each pair of cities should be taken into account in the sum exactly once, i. e. we count unordered pairs.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 300</span>) — amount of cities in Berland. Then there follow <span class="tex-span"><i>n</i></span> lines with <span class="tex-span"><i>n</i></span> integer numbers each — the matrix of shortest distances. <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th row — <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>, the shortest distance between cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>. It is guaranteed that <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0, <i>d</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = <i>d</i><sub class="lower-index"><i>j</i>, <i>i</i></sub></span>, and a given matrix is a matrix of shortest distances for some set of two-way roads with integer lengths from 1 to 1000, such that from each city it is possible to get to any other city using these roads.</p><p>Next line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 300</span>) — amount of planned roads. Following <span class="tex-span"><i>k</i></span> lines contain the description of the planned roads. Each road is described by three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — pair of cities, which the road connects, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the length of the road. It can be several roads between a pair of cities, but no road connects the city with itself.</p>

## Output

<p>Output <span class="tex-span"><i>k</i></span> space-separated integers <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>). <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> should be equal to the sum of shortest distances between all pairs of cities after the construction of roads with indexes from 1 to <span class="tex-span"><i>i</i></span>. Roads are numbered from 1 in the input order. Each pair of cities should be taken into account in the sum exactly once, i. e. we count unordered pairs.</p>





```input1
2
0 5
5 0
1
1 2 3

```




```input2
3
0 4 5
4 0 9
5 9 0
2
2 3 8
1 2 1

```




```output1
3
```




```output2
17 12
```


