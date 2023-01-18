## Description

<div><p>Life in Bertown has become hard. The city has too many roads and the government spends too much to maintain them. There are <span class="tex-span"><i>n</i></span> junctions and <span class="tex-span"><i>m</i></span> two way roads, at which one can get from each junction to any other one. The mayor wants to close some roads so that the number of roads left totaled to <span class="tex-span"><i>n</i> - 1</span> roads and it were still possible to get from each junction to any other one. Besides, the mayor is concerned with the number of dead ends which are the junctions from which only one road goes. There shouldn't be too many or too few junctions. Having discussed the problem, the mayor and his assistants decided that after the roads are closed, the road map should contain exactly <span class="tex-span"><i>k</i></span> dead ends. Your task is to count the number of different ways of closing the roads at which the following conditions are met: </p><ul> <li> There are exactly <span class="tex-span"><i>n</i> - 1</span> roads left. </li><li> It is possible to get from each junction to any other one. </li><li> There are exactly <span class="tex-span"><i>k</i></span> dead ends on the resulting map. </li></ul><p>Two ways are considered different if there is a road that is closed in the first way, and is open in the second one.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10, <i>n</i> - 1 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1) / 2, 2 ≤ <i>k</i> ≤ <i>n</i> - 1</span>) which represent the number of junctions, roads and dead ends correspondingly. Then follow <span class="tex-span"><i>m</i></span> lines each containing two different integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ <i>n</i>, <i>v</i><sub class="lower-index">1</sub> ≠ <i>v</i><sub class="lower-index">2</sub></span>) which represent the number of junctions connected by another road. There can be no more than one road between every pair of junctions. The junctions are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that it is possible to get from each junction to any other one along the original roads.</p></div><div class="output-specification"><p>Print a single number — the required number of ways.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10, <i>n</i> - 1 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1) / 2, 2 ≤ <i>k</i> ≤ <i>n</i> - 1</span>) which represent the number of junctions, roads and dead ends correspondingly. Then follow <span class="tex-span"><i>m</i></span> lines each containing two different integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ <i>n</i>, <i>v</i><sub class="lower-index">1</sub> ≠ <i>v</i><sub class="lower-index">2</sub></span>) which represent the number of junctions connected by another road. There can be no more than one road between every pair of junctions. The junctions are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that it is possible to get from each junction to any other one along the original roads.</p>

## Output

<p>Print a single number — the required number of ways.</p>





```input1
3 3 2
1 2
2 3
1 3

```




```input2
4 6 2
1 2
2 3
3 4
4 1
1 3
2 4

```




```input3
4 6 3
1 2
2 3
3 4
4 1
1 3
2 4

```




```output1
3

```




```output2
12

```




```output3
4

```


