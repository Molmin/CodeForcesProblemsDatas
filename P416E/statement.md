## Description

<div><p>Good old Berland has <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>m</i></span> roads. Each road connects a pair of distinct cities and is bidirectional. Between any pair of cities, there is at most one road. For each road, we know its length.</p><p>We also know that the President will soon ride along the Berland roads from city <span class="tex-span"><i>s</i></span> to city <span class="tex-span"><i>t</i></span>. Naturally, he will choose one of the shortest paths from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>, but nobody can say for sure which path he will choose.</p><p>The Minister for Transport is really afraid that the President might get upset by the state of the roads in the country. That is the reason he is planning to repair the roads in the possible President's path.</p><p>Making the budget for such an event is not an easy task. For all possible distinct pairs <span class="tex-span"><i>s</i>, <i>t</i></span> (<span class="tex-span"><i>s</i> &lt; <i>t</i></span>) find the number of roads that lie on at least one shortest path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1) / 2</span>) — the number of cities and roads, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow, containing the road descriptions, one description per line. Each description contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the cities connected by the <span class="tex-span"><i>i</i></span>-th road and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is its length.</p></div><div class="output-specification"><p>Print the sequence of <img align="middle" class="tex-formula" src="file://UbLRpePj.png" style="max-width: 100.0%;max-height: 100.0%;"> integers <span class="tex-span"><i>c</i><sub class="lower-index">12</sub>, <i>c</i><sub class="lower-index">13</sub>, ..., <i>c</i><sub class="lower-index">1<i>n</i></sub>, <i>c</i><sub class="lower-index">23</sub>, <i>c</i><sub class="lower-index">24</sub>, ..., <i>c</i><sub class="lower-index">2<i>n</i></sub>, ..., <i>c</i><sub class="lower-index"><i>n</i> - 1, <i>n</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>st</i></sub></span> is the number of roads that can lie on the shortest path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>. Print the elements of sequence <span class="tex-span"><i>c</i></span> in the described order. If the pair of cities <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> don't have a path between them, then <span class="tex-span"><i>c</i><sub class="lower-index"><i>st</i></sub> = 0</span>.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i>·(<i>n</i> - 1) / 2</span>) — the number of cities and roads, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow, containing the road descriptions, one description per line. Each description contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> are the numbers of the cities connected by the <span class="tex-span"><i>i</i></span>-th road and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is its length.</p>

## Output

<p>Print the sequence of <img align="middle" class="tex-formula" src="file://UbLRpePj.png" style="max-width: 100.0%;max-height: 100.0%;"> integers <span class="tex-span"><i>c</i><sub class="lower-index">12</sub>, <i>c</i><sub class="lower-index">13</sub>, ..., <i>c</i><sub class="lower-index">1<i>n</i></sub>, <i>c</i><sub class="lower-index">23</sub>, <i>c</i><sub class="lower-index">24</sub>, ..., <i>c</i><sub class="lower-index">2<i>n</i></sub>, ..., <i>c</i><sub class="lower-index"><i>n</i> - 1, <i>n</i></sub></span>, where <span class="tex-span"><i>c</i><sub class="lower-index"><i>st</i></sub></span> is the number of roads that can lie on the shortest path from <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span>. Print the elements of sequence <span class="tex-span"><i>c</i></span> in the described order. If the pair of cities <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> don't have a path between them, then <span class="tex-span"><i>c</i><sub class="lower-index"><i>st</i></sub> = 0</span>.</p>





```input1
5 6
1 2 1
2 3 1
3 4 1
4 1 1
2 4 2
4 5 4

```




```output1
1 4 1 2 1 5 6 1 2 1
```


