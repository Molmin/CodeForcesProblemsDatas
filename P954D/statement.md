## Description

<div><p>Little town Nsk consists of <span class="tex-span"><i>n</i></span> junctions connected by <span class="tex-span"><i>m</i></span> bidirectional roads. Each road connects two distinct junctions and no two roads connect the same pair of junctions. It is possible to get from any junction to any other junction by these roads. The distance between two junctions is equal to the minimum possible number of roads on a path between them.</p><p>In order to improve the transportation system, the city council asks mayor to build one new road. The problem is that the mayor has just bought a wonderful new car and he really enjoys a ride from his home, located near junction <span class="tex-span"><i>s</i></span> to work located near junction <span class="tex-span"><i>t</i></span>. Thus, he wants to build a new road in such a way that the distance between these two junctions won't decrease. </p><p>You are assigned a task to compute the number of pairs of junctions that are not connected by the road, such that if the new road between these two junctions is built the distance between <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> won't decrease.</p></div><div class="input-specification"><p>The firt line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i> ≠ <i>t</i></span>)&nbsp;— the number of junctions and the number of roads in Nsk, as well as the indices of junctions where mayors home and work are located respectively. The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), meaning that this road connects junctions <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> directly. It is guaranteed that there is a path between any two junctions and no two roads connect the same pair of junctions.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of pairs of junctions not connected by a direct road, such that building a road between these two junctions won't decrease the distance between junctions <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The firt line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>, <span class="tex-span"><i>s</i> ≠ <i>t</i></span>)&nbsp;— the number of junctions and the number of roads in Nsk, as well as the indices of junctions where mayors home and work are located respectively. The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>), meaning that this road connects junctions <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> directly. It is guaranteed that there is a path between any two junctions and no two roads connect the same pair of junctions.</p>

## Output

<p>Print one integer&nbsp;— the number of pairs of junctions not connected by a direct road, such that building a road between these two junctions won't decrease the distance between junctions <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>.</p>





```input1
5 4 1 5
1 2
2 3
3 4
4 5

```




```input2
5 4 3 5
1 2
2 3
3 4
4 5

```




```input3
5 6 1 5
1 2
1 3
1 4
4 5
3 5
2 5

```




```output1
0

```




```output2
5

```




```output3
3

```


