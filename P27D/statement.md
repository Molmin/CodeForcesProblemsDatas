## Description

<div><p>It is well known that Berland has <span class="tex-span"><i>n</i></span> cities, which form the Silver ring — cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>) are connected by a road, as well as the cities <span class="tex-span"><i>n</i></span> and <span class="tex-span">1</span>. The goverment have decided to build <span class="tex-span"><i>m</i></span> new roads. The list of the roads to build was prepared. Each road will connect two cities. Each road should be a curve which lies inside or outside the ring. New roads will have no common points with the ring (except the endpoints of the road).</p><p>Now the designers of the constructing plan wonder if it is possible to build the roads in such a way that no two roads intersect (note that the roads may intersect at their endpoints). If it is possible to do, which roads should be inside the ring, and which should be outside?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). No two cities will be connected by more than one road in the list. The list will not contain the roads which exist in the Silver ring.</p></div><div class="output-specification"><p>If it is impossible to build the roads in such a way that no two roads intersect, output <span class="tex-font-style-tt">Impossible</span>. Otherwise print <span class="tex-span"><i>m</i></span> characters. <span class="tex-span"><i>i</i></span>-th character should be <span class="tex-font-style-tt">i</span>, if the road should be inside the ring, and <span class="tex-font-style-tt">o</span> if the road should be outside the ring. If there are several solutions, output any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 100, 1 ≤ <i>m</i> ≤ 100</span>). Each of the following <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). No two cities will be connected by more than one road in the list. The list will not contain the roads which exist in the Silver ring.</p>

## Output

<p>If it is impossible to build the roads in such a way that no two roads intersect, output <span class="tex-font-style-tt">Impossible</span>. Otherwise print <span class="tex-span"><i>m</i></span> characters. <span class="tex-span"><i>i</i></span>-th character should be <span class="tex-font-style-tt">i</span>, if the road should be inside the ring, and <span class="tex-font-style-tt">o</span> if the road should be outside the ring. If there are several solutions, output any of them.</p>





```input1
4 2
1 3
2 4

```




```input2
6 3
1 3
3 5
5 1

```




```output1
io

```




```output2
ooo

```


