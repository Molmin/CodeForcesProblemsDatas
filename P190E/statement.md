## Description

<div><p>Berland has managed to repel the flatlanders' attack and is now starting the counter attack.</p><p>Flatland has <span class="tex-span"><i>n</i></span> cities, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and some pairs of them are connected by bidirectional roads. The Flatlandian maps show roads between cities if and only if there is in fact no road between this pair of cities (we do not know whether is it a clever spy-proof strategy or just saving ink). In other words, if two cities are connected by a road on a flatland map, then there is in fact no road between them. The opposite situation is also true: if two cities are not connected by a road on a flatland map, then in fact, there is a road between them.</p><p>The berlanders got hold of a flatland map. Now Vasya the Corporal is commissioned by General Touristov to find all such groups of flatland cities, that in each group of cities you can get from any city to any other one, moving along the <span class="tex-font-style-bf">actual</span> roads. Also the cities from different groups are unreachable from each other, moving along the <span class="tex-font-style-bf">actual</span> roads. Indeed, destroying such groups one by one is much easier than surrounding all Flatland at once!</p><p>Help the corporal complete this task and finally become a sergeant! Don't forget that a flatland map shows a road between cities if and only if there is in fact no road between them. </p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of cities and the number of roads marked on the flatland map, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain descriptions of the cities on the map. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers of cities that are connected by the <span class="tex-span"><i>i</i></span>-th road on the flatland map.</p><p>It is guaranteed that each pair of cities occurs in the input no more than once.</p></div><div class="output-specification"><p>On the first line print number <span class="tex-span"><i>k</i></span> — the number of groups of cities in Flatland, such that in each group you can get from any city to any other one by flatland roads. At the same time, the cities from different groups should be unreachable by flatland roads.</p><p>On each of the following <span class="tex-span"><i>k</i></span> lines first print <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the number of vertexes in the <span class="tex-span"><i>i</i></span>-th group. Then print space-separated numbers of cities in the <span class="tex-span"><i>i</i></span>-th group.</p><p>The order of printing groups and the order of printing numbers in the groups does not matter. The total sum <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>k</i></span> groups must equal <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>, 0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the number of cities and the number of roads marked on the flatland map, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain descriptions of the cities on the map. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> — the numbers of cities that are connected by the <span class="tex-span"><i>i</i></span>-th road on the flatland map.</p><p>It is guaranteed that each pair of cities occurs in the input no more than once.</p>

## Output

<p>On the first line print number <span class="tex-span"><i>k</i></span> — the number of groups of cities in Flatland, such that in each group you can get from any city to any other one by flatland roads. At the same time, the cities from different groups should be unreachable by flatland roads.</p><p>On each of the following <span class="tex-span"><i>k</i></span> lines first print <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the number of vertexes in the <span class="tex-span"><i>i</i></span>-th group. Then print space-separated numbers of cities in the <span class="tex-span"><i>i</i></span>-th group.</p><p>The order of printing groups and the order of printing numbers in the groups does not matter. The total sum <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>k</i></span> groups must equal <span class="tex-span"><i>n</i></span>.</p>





```input1
4 4
1 2
1 3
4 2
4 3

```




```input2
3 1
1 2

```




```output1
2
2 1 4 
2 2 3 

```




```output2
1
3 1 2 3 

```



## Note

<p>In the first sample there are roads only between pairs of cities 1-4 and 2-3.</p><p>In the second sample there is no road between cities 1 and 2, but still you can get from one city to the other one through city number 3.</p>
