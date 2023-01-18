## Description

<div><p>In Ancient Berland there were <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>m</i></span> two-way roads of equal length. The cities are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusively. According to an ancient superstition, if a traveller visits three cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> in row, without visiting other cities between them, a great disaster awaits him. Overall there are <span class="tex-span"><i>k</i></span> such city triplets. Each triplet is ordered, which means that, for example, you are allowed to visit the cities in the following order: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Vasya wants to get from the city <span class="tex-span">1</span> to the city <span class="tex-span"><i>n</i></span> and not fulfil the superstition. Find out which minimal number of roads he should take. Also you are required to find one of his possible path routes.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3000, 1 ≤ <i>m</i> ≤ 20000, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) which are the number of cities, the number of roads and the number of the forbidden triplets correspondingly. </p><p>Then follow <span class="tex-span"><i>m</i></span> lines each containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which are the road descriptions. The road is described by the numbers of the cities it joins. No road joins a city with itself, there cannot be more than one road between a pair of cities. </p><p>Then follow <span class="tex-span"><i>k</i></span> lines each containing three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which are the forbidden triplets. Each ordered triplet is listed mo more than one time. All three cities in each triplet are distinct.</p><p>City <span class="tex-span"><i>n</i></span> can be unreachable from city <span class="tex-span">1</span> by roads.</p></div><div class="output-specification"><p>If there are no path from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> print <span class="tex-font-style-tt">-1</span>. Otherwise on the first line print the number of roads <span class="tex-span"><i>d</i></span> along the shortest path from the city <span class="tex-span">1</span> to the city <span class="tex-span"><i>n</i></span>. On the second line print <span class="tex-span"><i>d</i> + 1</span> numbers — any of the possible shortest paths for Vasya. The path should start in the city <span class="tex-span">1</span> and end in the city <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3000, 1 ≤ <i>m</i> ≤ 20000, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) which are the number of cities, the number of roads and the number of the forbidden triplets correspondingly. </p><p>Then follow <span class="tex-span"><i>m</i></span> lines each containing two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which are the road descriptions. The road is described by the numbers of the cities it joins. No road joins a city with itself, there cannot be more than one road between a pair of cities. </p><p>Then follow <span class="tex-span"><i>k</i></span> lines each containing three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which are the forbidden triplets. Each ordered triplet is listed mo more than one time. All three cities in each triplet are distinct.</p><p>City <span class="tex-span"><i>n</i></span> can be unreachable from city <span class="tex-span">1</span> by roads.</p>

## Output

<p>If there are no path from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> print <span class="tex-font-style-tt">-1</span>. Otherwise on the first line print the number of roads <span class="tex-span"><i>d</i></span> along the shortest path from the city <span class="tex-span">1</span> to the city <span class="tex-span"><i>n</i></span>. On the second line print <span class="tex-span"><i>d</i> + 1</span> numbers — any of the possible shortest paths for Vasya. The path should start in the city <span class="tex-span">1</span> and end in the city <span class="tex-span"><i>n</i></span>.</p>





```input1
4 4 1
1 2
2 3
3 4
1 3
1 4 3

```




```input2
3 1 0
1 2

```




```input3
4 4 2
1 2
2 3
3 4
1 3
1 2 3
1 3 4

```




```output1
2
1 3 4

```




```output2
-1

```




```output3
4
1 3 2 3 4

```


