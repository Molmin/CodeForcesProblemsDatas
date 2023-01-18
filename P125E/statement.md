## Description

<div><p>The MST (Meaningless State Team) company won another tender for an important state reform in Berland.</p><p>There are <span class="tex-span"><i>n</i></span> cities in Berland, some pairs of the cities are connected by roads. Each road has its price. One can move along any road in any direction. The MST team should carry out the repair works on some set of roads such that one can get from any city to any other one moving only along the repaired roads. Moreover, this set should contain exactly <span class="tex-span"><i>k</i></span> capital roads (that is, the roads that start or finish in the capital). The number of the capital is 1.</p><p>As the budget has already been approved, the MST Company will profit by finding the set with minimum lengths of roads.</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;0 ≤ <i>k</i> &lt; 5000</span>), where <span class="tex-span"><i>n</i></span> is the number of cities in the country, <span class="tex-span"><i>m</i></span> is the number of roads in the country, <span class="tex-span"><i>k</i></span> is the number of capital roads in the required set. Then <span class="tex-span"><i>m</i></span> lines enumerate the roads in question. Each road is specified by three numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of cities linked by a road and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is its length. </p><p>Between each pair of cities no more than one road exists. There are no roads that start and finish in one city. The capital's number is 1.</p></div><div class="output-specification"><p>In the first line print the number of roads in the required set. The second line should contain the numbers of roads included in the sought set. If the sought set does not exist, print -1.</p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000;0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>;0 ≤ <i>k</i> &lt; 5000</span>), where <span class="tex-span"><i>n</i></span> is the number of cities in the country, <span class="tex-span"><i>m</i></span> is the number of roads in the country, <span class="tex-span"><i>k</i></span> is the number of capital roads in the required set. Then <span class="tex-span"><i>m</i></span> lines enumerate the roads in question. Each road is specified by three numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of cities linked by a road and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is its length. </p><p>Between each pair of cities no more than one road exists. There are no roads that start and finish in one city. The capital's number is 1.</p>

## Output

<p>In the first line print the number of roads in the required set. The second line should contain the numbers of roads included in the sought set. If the sought set does not exist, print -1.</p>





```input1
4 5 2
1 2 1
2 3 1
3 4 1
1 3 3
1 4 2

```




```output1
3
1 5 2
```


