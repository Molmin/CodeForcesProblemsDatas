## Description

<div><p>Nudist Beach is planning a military operation to attack the Life Fibers. In this operation, they will attack and capture several cities which are currently under the control of the Life Fibers.</p><p>There are <span class="tex-span"><i>n</i></span> cities, labeled from 1 to <span class="tex-span"><i>n</i></span>, and <span class="tex-span"><i>m</i></span> bidirectional roads between them. Currently, there are Life Fibers in every city. In addition, there are <span class="tex-span"><i>k</i></span> cities that are fortresses of the Life Fibers that cannot be captured under any circumstances. So, the Nudist Beach can capture an arbitrary non-empty subset of cities with no fortresses.</p><p>After the operation, Nudist Beach will have to defend the captured cities from counterattack. If they capture a city and it is connected to many Life Fiber controlled cities, it will be easily defeated. So, Nudist Beach would like to capture a set of cities such that for each captured city the ratio of Nudist Beach controlled neighbors among all neighbors of that city is as high as possible. </p><p>More formally, they would like to capture a non-empty set of cities <span class="tex-span"><i>S</i></span> with no fortresses of Life Fibers. The strength of a city <img align="middle" class="tex-formula" src="file://70ULpZhP.png" style="max-width: 100.0%;max-height: 100.0%;"> is defined as (number of neighbors of <span class="tex-span"><i>x</i></span> in <span class="tex-span"><i>S</i></span>) / (total number of neighbors of <span class="tex-span"><i>x</i></span>). Here, two cities are called neighbors if they are connnected with a road. The goal is to maximize the strength of the weakest city in <span class="tex-span"><i>S</i></span>.</p><p>Given a description of the graph, and the cities with fortresses, find a non-empty subset that maximizes the strength of the weakest city. </p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>).</p><p>The second line of input contains <span class="tex-span"><i>k</i></span> integers, representing the cities with fortresses. These cities will all be distinct. </p><p>The next <span class="tex-span"><i>m</i></span> lines contain the roads. The <span class="tex-span"><i>i</i></span>-th of these lines will have 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Every city will have at least one road adjacent to it.</p><p>There is no more than one road between each pair of the cities.</p></div><div class="output-specification"><p>The first line should contain an integer <span class="tex-span"><i>r</i></span>, denoting the size of an optimum set (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i> - <i>k</i></span>). </p><p>The second line should contain <span class="tex-span"><i>r</i></span> integers, denoting the cities in the set. Cities may follow in an arbitrary order. This line should not contain any of the cities with fortresses.</p><p>If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> - 1</span>).</p><p>The second line of input contains <span class="tex-span"><i>k</i></span> integers, representing the cities with fortresses. These cities will all be distinct. </p><p>The next <span class="tex-span"><i>m</i></span> lines contain the roads. The <span class="tex-span"><i>i</i></span>-th of these lines will have 2 integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Every city will have at least one road adjacent to it.</p><p>There is no more than one road between each pair of the cities.</p>

## Output

<p>The first line should contain an integer <span class="tex-span"><i>r</i></span>, denoting the size of an optimum set (<span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i> - <i>k</i></span>). </p><p>The second line should contain <span class="tex-span"><i>r</i></span> integers, denoting the cities in the set. Cities may follow in an arbitrary order. This line should not contain any of the cities with fortresses.</p><p>If there are multiple possible answers, print any of them.</p>





```input1
9 8 4
3 9 6 8
1 2
1 3
1 4
1 5
2 6
2 7
2 8
2 9

```




```input2
10 8 2
2 9
1 3
2 9
4 5
5 6
6 7
7 8
8 10
10 4

```




```output1
3
1 4 5

```




```output2
8
1 5 4 8 10 6 3 7

```



## Note

<p>The first example case achieves a strength of 1/2. No other subset is strictly better.</p><p>The second example case achieves a strength of 1. Note that the subset doesn't necessarily have to be connected.</p>
