## Description

<div><p>The Berland road network consists of <span class="tex-span"><i>n</i></span> cities and of <span class="tex-span"><i>m</i></span> bidirectional roads. The cities are numbered from 1 to <span class="tex-span"><i>n</i></span>, where the main capital city has number <span class="tex-span"><i>n</i></span>, and the culture capital — number <span class="tex-span">1</span>. The road network is set up so that it is possible to reach any city from any other one by the roads. Moving on each road in any direction takes the same time.</p><p>All residents of Berland are very lazy people, and so when they want to get from city <span class="tex-span"><i>v</i></span> to city <span class="tex-span"><i>u</i></span>, they always choose one of the shortest paths (no matter which one).</p><p>The Berland government wants to make this country's road network safer. For that, it is going to put a police station in one city. The police station has a rather strange property: when a citizen of Berland is driving along the road with a police station at one end of it, the citizen drives more carefully, so all such roads are considered safe. The roads, both ends of which differ from the city with the police station, are dangerous.</p><p>Now the government wonders where to put the police station so that the average number of safe roads for <span class="tex-font-style-bf">all</span> the shortest paths from the cultural capital to the main capital would take the maximum value.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <img align="middle" class="tex-formula" src="file://UzkNJIxD.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of cities and the number of roads in Berland, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>) — the numbers of cities that are connected by the <span class="tex-span"><i>i</i></span>-th road. The numbers on a line are separated by a space. </p><p>It is guaranteed that each pair of cities is connected with no more than one road and that it is possible to get from any city to any other one along Berland roads.</p></div><div class="output-specification"><p>Print the maximum possible value of the average number of safe roads among all shortest paths from the culture capital to the main one. The answer will be considered valid if its absolute or relative inaccuracy does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <img align="middle" class="tex-formula" src="file://UzkNJIxD.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of cities and the number of roads in Berland, correspondingly. Next <span class="tex-span"><i>m</i></span> lines contain pairs of integers <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>u</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> ≠ <i>u</i><sub class="lower-index"><i>i</i></sub></span>) — the numbers of cities that are connected by the <span class="tex-span"><i>i</i></span>-th road. The numbers on a line are separated by a space. </p><p>It is guaranteed that each pair of cities is connected with no more than one road and that it is possible to get from any city to any other one along Berland roads.</p>

## Output

<p>Print the maximum possible value of the average number of safe roads among all shortest paths from the culture capital to the main one. The answer will be considered valid if its absolute or relative inaccuracy does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4 4
1 2
2 4
1 3
3 4

```




```input2
11 14
1 2
1 3
2 4
3 4
4 5
4 6
5 11
6 11
1 8
8 9
9 7
11 7
1 10
10 4

```




```output1
1.000000000000

```




```output2
1.714285714286

```



## Note

<p>In the first sample you can put a police station in one of the capitals, then each path will have exactly one safe road. If we place the station not in the capital, then the average number of safe roads will also make <img align="middle" class="tex-formula" src="file://cpHU4KUC.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample we can obtain the maximum sought value if we put the station in city <span class="tex-span">4</span>, then <span class="tex-span">6</span> paths will have <span class="tex-span">2</span> safe roads each, and one path will have <span class="tex-span">0</span> safe roads, so the answer will equal <img align="middle" class="tex-formula" src="file://6zjlX6Z5.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
