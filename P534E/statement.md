## Description

<div><p>In Berland a bus travels along the main street of the capital. The street begins from the main square and looks like a very long segment. There are <span class="tex-span"><i>n</i></span> bus stops located along the street, the <span class="tex-span"><i>i</i></span>-th of them is located at the distance <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from the central square, all distances are distinct, the stops are numbered in the order of increasing distance from the square, that is, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i> - 1</span>. The bus starts its journey from the first stop, it passes stops <span class="tex-span">2</span>, <span class="tex-span">3</span> and so on. It reaches the stop number <span class="tex-span"><i>n</i></span>, turns around and goes in the opposite direction to stop <span class="tex-span">1</span>, passing all the intermediate stops in the reverse order. After that, it again starts to move towards stop <span class="tex-span"><i>n</i></span>. During the day, the bus runs non-stop on this route.</p><p>The bus is equipped with the Berland local positioning system. When the bus passes a stop, the system notes down its number.</p><p>One of the key features of the system is that it can respond to the queries about the distance covered by the bus for the parts of its path between some pair of stops. A special module of the system takes the input with the information about a set of stops on a segment of the path, a stop number occurs in the set as many times as the bus drove past it. This module returns the length of the traveled segment of the path (or -1 if it is impossible to determine the length uniquely). The operation of the module is complicated by the fact that <span class="tex-font-style-it">stop numbers occur in the request not in the order they were visited but in the non-decreasing order</span>.</p><p>For example, if the number of stops is <span class="tex-span">6</span>, and the part of the bus path starts at the bus stop number <span class="tex-span">5</span>, ends at the stop number <span class="tex-span">3</span> and passes the stops as follows: <img align="middle" class="tex-formula" src="file://ucRoyGNE.png" style="max-width: 100.0%;max-height: 100.0%;">, then the request about this segment of the path will have form: <span class="tex-span">3, 4, 5, 5, 6</span>. If the bus on the segment of the path from stop <span class="tex-span">5</span> to stop <span class="tex-span">3</span> has time to drive past the <span class="tex-span">1</span>-th stop (i.e., if we consider a segment that ends with the second visit to stop <span class="tex-span">3</span> on the way from <span class="tex-span">5</span>), then the request will have form: <span class="tex-span">1, 2, 2, 3, 3, 4, 5, 5, 6</span>.</p><p>You will have to repeat the Berland programmers achievement and implement this function.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of stops.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the distance from the <span class="tex-span"><i>i</i></span>-th stop to the central square. The numbers in the second line go in the increasing order.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 4·10<sup class="upper-index">5</sup></span>) — the number of stops the bus visited on some segment of the path.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sorted list of numbers of the stops visited by the bus on the segment of the path. The number of a stop occurs as many times as it was visited by a bus.</p><p>It is guaranteed that the query corresponds to some segment of the path.</p></div><div class="output-specification"><p>In the single line please print the distance covered by a bus. If it is impossible to determine it unambiguously, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of stops.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the distance from the <span class="tex-span"><i>i</i></span>-th stop to the central square. The numbers in the second line go in the increasing order.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 4·10<sup class="upper-index">5</sup></span>) — the number of stops the bus visited on some segment of the path.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sorted list of numbers of the stops visited by the bus on the segment of the path. The number of a stop occurs as many times as it was visited by a bus.</p><p>It is guaranteed that the query corresponds to some segment of the path.</p>

## Output

<p>In the single line please print the distance covered by a bus. If it is impossible to determine it unambiguously, print <span class="tex-span"> - 1</span>.</p>





```input1
6
2 3 5 7 11 13
5
3 4 5 5 6

```




```input2
6
2 3 5 7 11 13
9
1 2 2 3 3 4 5 5 6

```




```input3
3
10 200 300
4
1 2 2 3

```




```input4
3
1 2 3
4
1 2 2 3

```




```output1
10

```




```output2
16

```




```output3
-1

```




```output4
3

```



## Note

<p>The first test from the statement demonstrates the first example shown in the statement of the problem.</p><p>The second test from the statement demonstrates the second example shown in the statement of the problem.</p><p>In the third sample there are two possible paths that have distinct lengths, consequently, the sought length of the segment isn't defined uniquely.</p><p>In the fourth sample, even though two distinct paths correspond to the query, they have the same lengths, so the sought length of the segment is defined uniquely.</p>
