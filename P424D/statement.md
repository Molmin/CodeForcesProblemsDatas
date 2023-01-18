## Description

<div><p>Recently an official statement of the world Olympic Committee said that the Olympic Winter Games 2030 will be held in Tomsk. The city officials decided to prepare for the Olympics thoroughly and to build all the necessary Olympic facilities as early as possible. First, a biathlon track will be built.</p><p>To construct a biathlon track a plot of land was allocated, which is a rectangle divided into <span class="tex-span"><i>n</i> × <i>m</i></span> identical squares. Each of the squares has two coordinates: the number of the row (from 1 to <span class="tex-span"><i>n</i></span>), where it is located, the number of the column (from 1 to <span class="tex-span"><i>m</i></span>), where it is located. Also each of the squares is characterized by its height. During the sports the biathletes will have to move from one square to another. If a biathlete moves from a higher square to a lower one, he makes a descent. If a biathlete moves from a lower square to a higher one, he makes an ascent. If a biathlete moves between two squares with the same height, then he moves on flat ground.</p><p>The biathlon track should be a border of some rectangular area of the allocated land on which biathletes will move in the clockwise direction. It is known that on one move on flat ground an average biathlete spends <span class="tex-span"><i>t</i><sub class="lower-index"><i>p</i></sub></span> seconds, an ascent takes <span class="tex-span"><i>t</i><sub class="lower-index"><i>u</i></sub></span> seconds, a descent takes <span class="tex-span"><i>t</i><sub class="lower-index"><i>d</i></sub></span> seconds. The Tomsk Administration wants to choose the route so that the average biathlete passes it in as close to <span class="tex-span"><i>t</i></span> seconds as possible. In other words, the difference between time <span class="tex-span"><i>t</i><sub class="lower-index"><i>s</i></sub></span> of passing the selected track and <span class="tex-span"><i>t</i></span> should be minimum.</p><p>For a better understanding you can look at the first sample of the input data. In this sample <span class="tex-span"><i>n</i> = 6, <i>m</i> = 7</span>, and the administration wants the track covering time to be as close to <span class="tex-span"><i>t</i> = 48</span> seconds as possible, also, <span class="tex-span"><i>t</i><sub class="lower-index"><i>p</i></sub> = 3</span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>u</i></sub> = 6</span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>d</i></sub> = 2</span>. If we consider the rectangle shown on the image by arrows, the average biathlete can move along the boundary in a clockwise direction in exactly <span class="tex-span">48</span> seconds. The upper left corner of this track is located in the square with the row number <span class="tex-span">4</span>, column number <span class="tex-span">3</span> and the lower right corner is at square with row number <span class="tex-span">6</span>, column number <span class="tex-span">7</span>.</p><center> <img class="tex-graphics" src="file://aA1Hxkbt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Among other things the administration wants all sides of the rectangle which boundaries will be the biathlon track to consist of no less than three squares and to be completely contained within the selected land.</p><p>You are given the description of the given plot of land and all necessary time values. You are to write the program to find the most suitable rectangle for a biathlon track. If there are several such rectangles, you are allowed to print any of them.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>) — the sizes of the land plot and the desired distance covering time.</p><p>The second line also contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>p</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>u</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>d</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>p</i></sub>, <i>t</i><sub class="lower-index"><i>u</i></sub>, <i>t</i><sub class="lower-index"><i>d</i></sub> ≤ 100</span>) — the time the average biathlete needs to cover a flat piece of the track, an ascent and a descent respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains <span class="tex-span"><i>m</i></span> integers that set the heights of each square of the given plot of land. Each of the height values is a positive integer, not exceeding <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>In a single line of the output print four positive integers — the number of the row and the number of the column of the upper left corner and the number of the row and the number of the column of the lower right corner of the rectangle that is chosen for the track.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>) — the sizes of the land plot and the desired distance covering time.</p><p>The second line also contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>p</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>u</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>d</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>p</i></sub>, <i>t</i><sub class="lower-index"><i>u</i></sub>, <i>t</i><sub class="lower-index"><i>d</i></sub> ≤ 100</span>) — the time the average biathlete needs to cover a flat piece of the track, an ascent and a descent respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains <span class="tex-span"><i>m</i></span> integers that set the heights of each square of the given plot of land. Each of the height values is a positive integer, not exceeding <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>In a single line of the output print four positive integers — the number of the row and the number of the column of the upper left corner and the number of the row and the number of the column of the lower right corner of the rectangle that is chosen for the track.</p>





```input1
6 7 48
3 6 2
5 4 8 3 3 7 9
4 1 6 8 7 1 1
1 6 4 6 4 8 6
7 2 6 1 6 9 4
1 9 8 6 3 9 2
4 5 6 8 4 3 7
```




```output1
4 3 6 7

```


