## Description

<div><p>Imagine a city with <span class="tex-span"><i>n</i></span> junctions and <span class="tex-span"><i>m</i></span> streets. Junctions are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>In order to increase the traffic flow, mayor of the city has decided to make each street one-way. This means in the street between junctions <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, the traffic moves only from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> or only from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>u</i></span>. </p><p>The problem is to direct the traffic flow of streets in a way that maximizes the number of pairs <span class="tex-span">(<i>u</i>, <i>v</i>)</span> where <span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i></span> and it is possible to reach junction <span class="tex-span"><i>v</i></span> from <span class="tex-span"><i>u</i></span> by passing the streets in their specified direction. Your task is to find out maximal possible number of such pairs.</p></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, (<img align="middle" class="tex-formula" src="file://26fKXEux.png" style="max-width: 100.0%;max-height: 100.0%;">), denoting the number of junctions and streets of the city.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, (<span class="tex-span"><i>u</i> ≠ <i>v</i></span>), denoting endpoints of a street in the city.</p><p>Between every two junctions there will be at most one street. It is guaranteed that before mayor decision (when all streets were two-way) it was possible to reach each junction from any other junction.</p></div><div class="output-specification"><p>Print the maximal number of pairs <span class="tex-span">(<i>u</i>, <i>v</i>)</span> such that that it is possible to reach junction <span class="tex-span"><i>v</i></span> from <span class="tex-span"><i>u</i></span> after directing the streets.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, (<img align="middle" class="tex-formula" src="file://26fKXEux.png" style="max-width: 100.0%;max-height: 100.0%;">), denoting the number of junctions and streets of the city.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>, (<span class="tex-span"><i>u</i> ≠ <i>v</i></span>), denoting endpoints of a street in the city.</p><p>Between every two junctions there will be at most one street. It is guaranteed that before mayor decision (when all streets were two-way) it was possible to reach each junction from any other junction.</p>

## Output

<p>Print the maximal number of pairs <span class="tex-span">(<i>u</i>, <i>v</i>)</span> such that that it is possible to reach junction <span class="tex-span"><i>v</i></span> from <span class="tex-span"><i>u</i></span> after directing the streets.</p>





```input1
5 4
1 2
1 3
1 4
1 5

```




```input2
4 5
1 2
2 3
3 4
4 1
1 3

```




```input3
2 1
1 2

```




```input4
6 7
1 2
2 3
1 3
1 4
4 5
5 6
6 4

```




```output1
13

```




```output2
16

```




```output3
3

```




```output4
27

```



## Note

<p>In the first sample, if the mayor makes first and second streets one-way towards the junction <span class="tex-span">1</span> and third and fourth streets in opposite direction, there would be 13 pairs of reachable junctions: <span class="tex-span">{(1, 1), (2, 2), (3, 3), (4, 4), (5, 5), (2, 1), (3, 1), (1, 4), (1, 5), (2, 4), (2, 5), (3, 4), (3, 5)}</span></p>
