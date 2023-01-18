## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities in Cyberland, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, connected by <span class="tex-span"><i>m</i></span> bidirectional roads. The <span class="tex-span"><i>j</i></span>-th road connects city <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>For tourists, souvenirs are sold in every city of Cyberland. In particular, city <span class="tex-span"><i>i</i></span> sell it at a price of <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Now there are <span class="tex-span"><i>q</i></span> queries for you to handle. There are two types of queries:</p><ul><li> "<span class="tex-font-style-tt">C <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>w</i></span></span>": The price in city <span class="tex-span"><i>a</i></span> is changed to <span class="tex-span"><i>w</i></span>.</li><li> "<span class="tex-font-style-tt">A <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span></span>": Now a tourist will travel from city <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>. He will choose a route, he also doesn't want to visit a city twice. He will buy souvenirs at the city where the souvenirs are the cheapest (possibly exactly at city <span class="tex-span"><i>a</i></span> or <span class="tex-span"><i>b</i></span>). You should output the minimum possible price that he can buy the souvenirs during his travel.</li></ul><p>More formally, we can define routes as follow:</p><ul><li> A route is a sequence of cities <span class="tex-span">[<i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub>]</span>, where <span class="tex-span"><i>k</i></span> is a certain positive integer.</li><li> For any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>k</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>x</i><sub class="lower-index"><i>j</i></sub></span>.</li><li> For any <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>, there is a road connecting <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</li><li> The minimum price of the route is <span class="tex-span"><i>min</i>(<i>w</i><sub class="lower-index"><i>x</i><sub class="lower-index">1</sub></sub>, <i>w</i><sub class="lower-index"><i>x</i><sub class="lower-index">2</sub></sub>, ..., <i>w</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>k</i></sub></sub>)</span>.</li><li> The required answer is the minimum value of the minimum prices of all valid routes from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span>.</li></ul></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), separated by a single space.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>j</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>).</p><p>It is guaranteed that there is at most one road connecting the same pair of cities. There is always at least one valid route between any two cities.</p><p>Next <span class="tex-span"><i>q</i></span> lines each describe a query. The format is "<span class="tex-font-style-tt">C <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>w</i></span></span>" or "<span class="tex-font-style-tt">A <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span></span>" (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>For each query of type "<span class="tex-font-style-tt">A</span>", output the corresponding answer.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), separated by a single space.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines contain pairs of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>j</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>).</p><p>It is guaranteed that there is at most one road connecting the same pair of cities. There is always at least one valid route between any two cities.</p><p>Next <span class="tex-span"><i>q</i></span> lines each describe a query. The format is "<span class="tex-font-style-tt">C <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>w</i></span></span>" or "<span class="tex-font-style-tt">A <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span></span>" (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, 1 ≤ <i>w</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>For each query of type "<span class="tex-font-style-tt">A</span>", output the corresponding answer.</p>





```input1
3 3 3
1
2
3
1 2
2 3
1 3
A 2 3
C 1 5
A 2 3

```




```input2
7 9 4
1
2
3
4
5
6
7
1 2
2 5
1 5
2 3
3 4
2 4
5 6
6 7
5 7
A 2 3
A 6 4
A 6 7
A 3 3

```




```output1
1
2

```




```output2
2
1
5
3

```



## Note

<p>For the second sample, an optimal routes are:</p><p>From <span class="tex-span">2</span> to <span class="tex-span">3</span> it is <span class="tex-span">[2, 3]</span>.</p><p>From <span class="tex-span">6</span> to <span class="tex-span">4</span> it is <span class="tex-span">[6, 5, 1, 2, 4]</span>.</p><p>From <span class="tex-span">6</span> to <span class="tex-span">7</span> it is <span class="tex-span">[6, 5, 7]</span>.</p><p>From <span class="tex-span">3</span> to <span class="tex-span">3</span> it is <span class="tex-span">[3]</span>.</p><center> <img class="tex-graphics" src="file://2jylqPxD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
