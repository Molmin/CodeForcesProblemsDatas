## Description

<div><p>A new trade empire is rising in Berland. Bulmart, an emerging trade giant, decided to dominate the market of ... shovels! And now almost every city in Berland has a Bulmart store, and some cities even have several of them! The only problem is, at the moment sales are ... let's say a little below estimates. Some people even say that shovels retail market is too small for such a big company to make a profit. But the company management believes in the future of that market and seeks new ways to increase income. </p><p>There are <span class="tex-span"><i>n</i></span> cities in Berland connected with <span class="tex-span"><i>m</i></span> bi-directional roads. All roads have equal lengths. It can happen that it is impossible to reach a city from another city using only roads. There is no road which connects a city to itself. Any pair of cities can be connected by at most one road.</p><p>There are <span class="tex-span"><i>w</i></span> Bulmart stores in Berland. Each of them is described by three numbers: </p><ul> <li> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — the number of city where the <span class="tex-span"><i>i</i></span>-th store is located (a city can have no stores at all or have several of them), </li><li> <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> — the number of shovels in the <span class="tex-span"><i>i</i></span>-th store, </li><li> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — the price of a single shovel in the <span class="tex-span"><i>i</i></span>-th store (in burles). </li></ul><p>The latest idea of the Bulmart management is to create a program which will help customers get shovels as fast as possible for affordable budget. Formally, the program has to find the minimum amount of time needed to deliver <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> shovels to the customer in the city <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub></span> for the total cost of no more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> burles. The delivery time between any two adjacent cities is equal to <span class="tex-span">1</span>. If shovels are delivered from several cities, the delivery time is equal to the arrival time of the last package. The delivery itself is free of charge.</p><p>The program needs to find answers to <span class="tex-span"><i>q</i></span> such queries. Each query has to be processed independently from others, i.e. a query does not change number of shovels in stores for the next queries.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>min</i>(5000, <i>n</i>·(<i>n</i> - 1) / 2))</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>e</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>e</i></sub></span>, meaning that the <span class="tex-span"><i>e</i></span>-th road connects cities <span class="tex-span"><i>x</i><sub class="lower-index"><i>e</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>e</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>e</i></sub>, <i>y</i><sub class="lower-index"><i>e</i></sub> ≤ <i>n</i></span>).</p><p>The next line contains a single integer <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>w</i> ≤ 5000</span>) — the total number of Bulmart stores in Berland. Each of the next <span class="tex-span"><i>w</i></span> lines contains three integers describing the <span class="tex-span"><i>i</i></span>-th store: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 1000</span>) — the number of queries. Each of the next <span class="tex-span"><i>q</i></span> lines contains three integers describing the <span class="tex-span"><i>j</i></span>-th query: <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>j</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> lines. On the <span class="tex-span"><i>j</i></span>-th line, print an answer for the <span class="tex-span"><i>j</i></span>-th query — the minimum amount of time needed to deliver <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> shovels to the customer in city <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub></span> spending no more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> burles. Print <span class="tex-font-style-tt">-1</span> if there is no solution for the <span class="tex-span"><i>j</i></span>-th query.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>min</i>(5000, <i>n</i>·(<i>n</i> - 1) / 2))</span>. Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>e</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>e</i></sub></span>, meaning that the <span class="tex-span"><i>e</i></span>-th road connects cities <span class="tex-span"><i>x</i><sub class="lower-index"><i>e</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>e</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>e</i></sub>, <i>y</i><sub class="lower-index"><i>e</i></sub> ≤ <i>n</i></span>).</p><p>The next line contains a single integer <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>w</i> ≤ 5000</span>) — the total number of Bulmart stores in Berland. Each of the next <span class="tex-span"><i>w</i></span> lines contains three integers describing the <span class="tex-span"><i>i</i></span>-th store: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, 1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The next line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 1000</span>) — the number of queries. Each of the next <span class="tex-span"><i>q</i></span> lines contains three integers describing the <span class="tex-span"><i>j</i></span>-th query: <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>j</i></sub>, <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> lines. On the <span class="tex-span"><i>j</i></span>-th line, print an answer for the <span class="tex-span"><i>j</i></span>-th query — the minimum amount of time needed to deliver <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span> shovels to the customer in city <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub></span> spending no more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> burles. Print <span class="tex-font-style-tt">-1</span> if there is no solution for the <span class="tex-span"><i>j</i></span>-th query.</p>





```input1
6 4
4 2
5 4
1 2
3 2
2
4 1 2
3 2 3
6
1 2 6
2 3 7
3 1 2
4 3 8
5 2 5
6 1 10

```




```output1
2
-1
2
2
3
-1

```


