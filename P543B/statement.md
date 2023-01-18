## Description

<div><p>In some country there are exactly <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>m</i></span> bidirectional roads connecting the cities. Cities are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. If cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are connected by a road, then in an hour you can go along this road either from city <span class="tex-span"><i>a</i></span> to city <span class="tex-span"><i>b</i></span>, or from city <span class="tex-span"><i>b</i></span> to city <span class="tex-span"><i>a</i></span>. The road network is such that from any city you can get to any other one by moving along the roads.</p><p>You want to destroy the largest possible number of roads in the country so that the remaining roads would allow you to get from city <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> to city <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> in at most <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> hours and get from city <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> to city <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> in at most <span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span> hours.</p><p>Determine what maximum number of roads you need to destroy in order to meet the condition of your plan. If it is impossible to reach the desired result, print -1.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>, <img align="middle" class="tex-formula" src="file://1oxepuci.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of cities and roads in the country, respectively. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the roads as pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that the roads that are given in the description can transport you from any city to any other one. It is guaranteed that each pair of cities has at most one road between them.</p><p>The last two lines contains three integers each, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span>, respectively (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print a single number — the answer to the problem. If the it is impossible to meet the conditions, print -1.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3000</span>, <img align="middle" class="tex-formula" src="file://1oxepuci.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of cities and roads in the country, respectively. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the roads as pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). It is guaranteed that the roads that are given in the description can transport you from any city to any other one. It is guaranteed that each pair of cities has at most one road between them.</p><p>The last two lines contains three integers each, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span>, respectively (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print a single number — the answer to the problem. If the it is impossible to meet the conditions, print -1.</p>





```input1
5 4
1 2
2 3
3 4
4 5
1 3 2
3 5 2

```




```input2
5 4
1 2
2 3
3 4
4 5
1 3 2
2 4 2

```




```input3
5 4
1 2
2 3
3 4
4 5
1 3 2
3 5 1

```




```output1
0

```




```output2
1

```




```output3
-1

```


