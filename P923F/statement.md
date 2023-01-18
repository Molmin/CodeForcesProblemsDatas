## Description

<div><p>There are <span class="tex-span"><i>N</i></span> cities in Bob's country connected by roads. Some pairs of cities are connected by public transport. There are two competing transport companies&nbsp;— <span class="tex-font-style-bf">Boblines</span> operating buses and <span class="tex-font-style-bf">Bobrail</span> running trains. When traveling from <span class="tex-span"><i>A</i></span> to <span class="tex-span"><i>B</i></span>, a passenger always first selects the mode of transport (either bus or train), and then embarks on a journey. For every pair of cities, there are exactly two ways of how to travel between them without visiting any city more than once&nbsp;— one using only bus routes, and the second using only train routes. Furthermore, there is no pair of cities that is directly connected by both a bus route and a train route.</p><p>You obtained the plans of each of the networks. Unfortunately, each of the companies uses different names for the same cities. More precisely, the bus company numbers the cities using integers from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span>, while the train company uses integers between <span class="tex-span"><i>N</i> + 1</span> and <span class="tex-span">2<i>N</i></span>. Find one possible mapping between those two numbering schemes, such that no pair of cities is connected directly by both a bus route and a train route. Note that this mapping has to map different cities to different cities.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 10000</span>), the number of cities.</p><p><span class="tex-span"><i>N</i> - 1</span> lines follow, representing the network plan of Boblines. Each contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>N</i></span>), meaning that there is a bus route between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p><span class="tex-span"><i>N</i> - 1</span> lines follow, representing the network plan of Bobrail. Each contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>N</i> + 1 ≤ <i>u</i>, <i>v</i> ≤ 2<i>N</i></span>), meaning that there is a train route between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p></div><div class="output-specification"><p>If there is no solution, output a single line with the word "<span class="tex-font-style-tt">No</span>".</p><p>If a solution exists, output two lines. On the first line, there should be the word "<span class="tex-font-style-tt">Yes</span>". On the second line, there should be <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>P</i><sub class="lower-index">1</sub>, <i>P</i><sub class="lower-index">2</sub>, ..., <i>P</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span"><i>N</i> + 1 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>N</i></span>)&nbsp;— the mapping between the two numbering schemes. More precisely, for <span class="tex-span"><i>i</i> ≠ <i>j</i></span> it should be <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub> ≠ <i>P</i><sub class="lower-index"><i>j</i></sub></span>, and for every direct bus route <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, there is no direct train route between <span class="tex-span">(<i>P</i><sub class="lower-index"><i>i</i></sub>, <i>P</i><sub class="lower-index"><i>j</i></sub>)</span>.</p><p>If there are multiple solutions, you may print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>N</i></span> (<span class="tex-span">2 ≤ <i>N</i> ≤ 10000</span>), the number of cities.</p><p><span class="tex-span"><i>N</i> - 1</span> lines follow, representing the network plan of Boblines. Each contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>u</i>, <i>v</i> ≤ <i>N</i></span>), meaning that there is a bus route between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p><span class="tex-span"><i>N</i> - 1</span> lines follow, representing the network plan of Bobrail. Each contains two integers <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>N</i> + 1 ≤ <i>u</i>, <i>v</i> ≤ 2<i>N</i></span>), meaning that there is a train route between cities <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p>

## Output

<p>If there is no solution, output a single line with the word "<span class="tex-font-style-tt">No</span>".</p><p>If a solution exists, output two lines. On the first line, there should be the word "<span class="tex-font-style-tt">Yes</span>". On the second line, there should be <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>P</i><sub class="lower-index">1</sub>, <i>P</i><sub class="lower-index">2</sub>, ..., <i>P</i><sub class="lower-index"><i>N</i></sub></span> (<span class="tex-span"><i>N</i> + 1 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> ≤ 2<i>N</i></span>)&nbsp;— the mapping between the two numbering schemes. More precisely, for <span class="tex-span"><i>i</i> ≠ <i>j</i></span> it should be <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub> ≠ <i>P</i><sub class="lower-index"><i>j</i></sub></span>, and for every direct bus route <span class="tex-span">(<i>i</i>, <i>j</i>)</span>, there is no direct train route between <span class="tex-span">(<i>P</i><sub class="lower-index"><i>i</i></sub>, <i>P</i><sub class="lower-index"><i>j</i></sub>)</span>.</p><p>If there are multiple solutions, you may print any of them.</p>





```input1
4
1 2
2 3
3 4
5 6
6 7
7 8

```




```input2
4
1 2
2 3
3 4
5 6
5 7
5 8

```




```input3
7
1 2
1 3
1 4
1 5
5 6
6 7
8 9
9 10
10 11
11 12
12 13
13 14

```




```output1
Yes
6 8 5 7

```




```output2
No

```




```output3
Yes
9 14 11 12 13 10 8

```



## Note

<p>The first sample (bus lines in red and rail lines in blue):</p><p><img class="tex-graphics" src="file://epI5vjVj.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
