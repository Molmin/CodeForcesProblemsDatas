## Description

<div><p>Berland has <span class="tex-span"><i>n</i></span> cities, the capital is located in city <span class="tex-span"><i>s</i></span>, and the historic home town of the President is in city <span class="tex-span"><i>t</i></span> (<span class="tex-span"><i>s</i> ≠ <i>t</i></span>). The cities are connected by one-way roads, the travel time for each of the road is a positive integer.</p><p>Once a year the President visited his historic home town <span class="tex-span"><i>t</i></span>, for which his motorcade passes along some path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span> (he always returns on a personal plane). Since the president is a very busy man, he always chooses the path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>, along which he will travel the fastest.</p><p>The ministry of Roads and Railways wants to learn for each of the road: whether the President will definitely pass through it during his travels, and if not, whether it is possible to repair it so that it would definitely be included in the shortest path from the capital to the historic home town of the President. Obviously, the road can not be repaired so that the travel time on it was less than one. The ministry of Berland, like any other, is interested in maintaining the budget, so it wants to know the minimum cost of repairing the road. Also, it is very fond of accuracy, so it repairs the roads so that the travel time on them is always a positive integer.</p></div><div class="input-specification"><p>The first lines contain four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>) — the number of cities and roads in Berland, the numbers of the capital and of the Presidents' home town (<span class="tex-span"><i>s</i> ≠ <i>t</i></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the roads. Each road is given as a group of three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the cities that are connected by the <span class="tex-span"><i>i</i></span>-th road and the time needed to ride along it. The road is directed from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The cities are numbered from 1 to <span class="tex-span"><i>n</i></span>. Each pair of cities can have multiple roads between them. It is guaranteed that there is a path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span> along the roads.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain information about the <span class="tex-span"><i>i</i></span>-th road (the roads are numbered in the order of appearance in the input).</p><p>If the president will definitely ride along it during his travels, the line must contain a single word "<span class="tex-font-style-tt">YES</span>" (without the quotes).</p><p>Otherwise, if the <span class="tex-span"><i>i</i></span>-th road can be repaired so that the travel time on it remains positive and then president will definitely ride along it, print space-separated word "<span class="tex-font-style-tt">CAN</span>" (without the quotes), and the minimum cost of repairing.</p><p>If <span class="tex-font-style-bf">we can't make the road be such that president will definitely ride along it</span>, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first lines contain four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>s</i>, <i>t</i> ≤ <i>n</i></span>) — the number of cities and roads in Berland, the numbers of the capital and of the Presidents' home town (<span class="tex-span"><i>s</i> ≠ <i>t</i></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain the roads. Each road is given as a group of three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the cities that are connected by the <span class="tex-span"><i>i</i></span>-th road and the time needed to ride along it. The road is directed from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The cities are numbered from 1 to <span class="tex-span"><i>n</i></span>. Each pair of cities can have multiple roads between them. It is guaranteed that there is a path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span> along the roads.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain information about the <span class="tex-span"><i>i</i></span>-th road (the roads are numbered in the order of appearance in the input).</p><p>If the president will definitely ride along it during his travels, the line must contain a single word "<span class="tex-font-style-tt">YES</span>" (without the quotes).</p><p>Otherwise, if the <span class="tex-span"><i>i</i></span>-th road can be repaired so that the travel time on it remains positive and then president will definitely ride along it, print space-separated word "<span class="tex-font-style-tt">CAN</span>" (without the quotes), and the minimum cost of repairing.</p><p>If <span class="tex-font-style-bf">we can't make the road be such that president will definitely ride along it</span>, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
6 7 1 6
1 2 2
1 3 10
2 3 7
2 4 8
3 5 3
4 5 2
5 6 1

```




```input2
3 3 1 3
1 2 10
2 3 10
1 3 100

```




```input3
2 2 1 2
1 2 1
1 2 2

```




```output1
YES
CAN 2
CAN 1
CAN 1
CAN 1
CAN 1
YES

```




```output2
YES
YES
CAN 81

```




```output3
YES
NO

```



## Note

<p>The cost of repairing the road is the difference between the time needed to ride along it before and after the repairing.</p><p>In the first sample president initially may choose one of the two following ways for a ride: <span class="tex-span">1 → 2 → 4 → 5 → 6</span> or <span class="tex-span">1 → 2 → 3 → 5 → 6</span>.</p>
