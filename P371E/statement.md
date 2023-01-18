## Description

<div><p>Berland is going through tough times — the dirt price has dropped and that is a blow to the country's economy. Everybody knows that Berland is the top world dirt exporter!</p><p>The President of Berland was forced to leave only <span class="tex-span"><i>k</i></span> of the currently existing <span class="tex-span"><i>n</i></span> subway stations.</p><p>The subway stations are located on a straight line one after another, the trains consecutively visit the stations as they move. You can assume that the stations are on the <span class="tex-span"><i>Ox</i></span> axis, the <span class="tex-span"><i>i</i></span>-th station is at point with coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. In such case the distance between stations <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> is calculated by a simple formula <span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>j</i></sub>|</span>.</p><p>Currently, the Ministry of Transport is choosing which stations to close and which ones to leave. Obviously, the residents of the capital won't be too enthusiastic about the innovation, so it was decided to show the best side to the people. The Ministry of Transport wants to choose such <span class="tex-span"><i>k</i></span> stations that minimize the average commute time in the subway!</p><p>Assuming that the train speed is constant (it is a fixed value), the average commute time in the subway is calculated as the sum of pairwise distances between stations, divided by the number of pairs (that is <img align="middle" class="tex-formula" src="file://pr3sqaWd.png" style="max-width: 100.0%;max-height: 100.0%;">) and divided by the speed of the train.</p><p>Help the Minister of Transport to solve this difficult problem. Write a program that, given the location of the stations selects such <span class="tex-span"><i>k</i></span> stations that the average commute time in the subway is minimized.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of the stations before the innovation. The second line contains the coordinates of the stations <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>). The third line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> - 1</span>) — the number of stations after the innovation.</p><p>The station coordinates are distinct and not necessarily sorted.</p></div><div class="output-specification"><p>Print a sequence of <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the numbers of the stations that should be left after the innovation in arbitrary order. Assume that the stations are numbered 1 through <span class="tex-span"><i>n</i></span> in the order they are given in the input. The number of stations you print must have the minimum possible average commute time among all possible ways to choose <span class="tex-span"><i>k</i></span> stations. If there are multiple such ways, you are allowed to print any of them.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of the stations before the innovation. The second line contains the coordinates of the stations <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>). The third line contains integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> - 1</span>) — the number of stations after the innovation.</p><p>The station coordinates are distinct and not necessarily sorted.</p>

## Output

<p>Print a sequence of <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the numbers of the stations that should be left after the innovation in arbitrary order. Assume that the stations are numbered 1 through <span class="tex-span"><i>n</i></span> in the order they are given in the input. The number of stations you print must have the minimum possible average commute time among all possible ways to choose <span class="tex-span"><i>k</i></span> stations. If there are multiple such ways, you are allowed to print any of them.</p>





```input1
3
1 100 101
2

```




```output1
2 3
```



## Note

<p>In the sample testcase the optimal answer is to destroy the first station (with <span class="tex-span"><i>x</i> = 1</span>). The average commute time will be equal to 1 in this way.</p>
