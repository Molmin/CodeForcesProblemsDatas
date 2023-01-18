## Description

<div><p>BerDonalds, a well-known fast food restaurant, is going to open a cafe in Bertown. The important thing is to choose the new restaurant's location so that it would be easy to get there. The Bertown road system is represented by <span class="tex-span"><i>n</i></span> junctions, connected by <span class="tex-span"><i>m</i></span> bidirectional roads. For each road we know its length. We also know that we can get from any junction to any other one, moving along the roads.</p><p>Your task is to find such location of the restaurant, that the shortest distance along the roads from the cafe to the farthest junction would be minimum. Note that the restaurant can be located not only on the junction, but at any point of any road.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://gQdgVGWw.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of junctions and the number of roads, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow, describing all Bertown roads. Each road is described by three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the junctions, connected by the <span class="tex-span"><i>i</i></span>-th road, and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the length of the <span class="tex-span"><i>i</i></span>-th road. </p><p>It is guaranteed that each road connects two distinct junctions, there is at most one road between any two junctions, and you can get from any junction to any other one.</p></div><div class="output-specification"><p>Print a single real number — the shortest distance from the optimal restaurant location to the farthest junction. The answer will be considered correct, if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://gQdgVGWw.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of junctions and the number of roads, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow, describing all Bertown roads. Each road is described by three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the junctions, connected by the <span class="tex-span"><i>i</i></span>-th road, and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the length of the <span class="tex-span"><i>i</i></span>-th road. </p><p>It is guaranteed that each road connects two distinct junctions, there is at most one road between any two junctions, and you can get from any junction to any other one.</p>

## Output

<p>Print a single real number — the shortest distance from the optimal restaurant location to the farthest junction. The answer will be considered correct, if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
2 1
1 2 1

```




```input2
3 3
1 2 1
2 3 1
1 3 1

```




```input3
3 2
1 2 100
2 3 1

```




```output1
0.50

```




```output2
1.00

```




```output3
50.50

```


