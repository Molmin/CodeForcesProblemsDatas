## Description

<div><p>Berland is a tourist country! At least, it can become such&nbsp;— the government of Berland is confident about this. </p><p>There are <span class="tex-span"><i>n</i></span> cities in Berland, some pairs of which are connected by two-ways roads. Each road connects two different cities. In Berland there are no roads which connect the same pair of cities. It is possible to get from any city to any other city using given two-ways roads. </p><p>According to the reform each road will become one-way. It will be oriented to one of two directions.</p><p>To maximize the tourist attraction of Berland, after the reform for each city <span class="tex-span"><i>i</i></span> the value <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> will be calculated. It will equal to the number of cities <span class="tex-span"><i>x</i></span> for which there is an oriented path from the city <span class="tex-span"><i>i</i></span> to the city <span class="tex-span"><i>x</i></span>. In other words, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> will equal the number of cities which can be reached from the city <span class="tex-span"><i>i</i></span> by roads. </p><p>The government is sure that tourist's attention will be focused on the minimum value of <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Help the government of Berland make the reform to maximize the minimum of <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400 000, 1 ≤ <i>m</i> ≤ 400 000</span>)&nbsp;— the number of cities and the number of roads. </p><p>The next <span class="tex-span"><i>m</i></span> lines describe roads in Berland: the <span class="tex-span"><i>j</i></span>-th of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub></span>), where <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> are the numbers of cities which are connected by the <span class="tex-span"><i>j</i></span>-th road.</p><p>The cities are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that it is possible to get from any city to any other by following two-ways roads. In Berland there are no roads which connect the same pair of cities. </p></div><div class="output-specification"><p>In the first line print single integer&nbsp;— the maximum possible value <span class="tex-span"><i>min</i><sub class="lower-index">1 ≤ <i>i</i> ≤ <i>n</i></sub>{<i>r</i><sub class="lower-index"><i>i</i></sub>}</span> after the orientation of roads. </p><p>The next <span class="tex-span"><i>m</i></span> lines must contain the description of roads after the orientation: the <span class="tex-span"><i>j</i></span>-th of them must contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub></span>, it means that the <span class="tex-span"><i>j</i></span>-th road will be directed from the city <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> to the city <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span>. Print roads in the same order as they are given in the input data. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400 000, 1 ≤ <i>m</i> ≤ 400 000</span>)&nbsp;— the number of cities and the number of roads. </p><p>The next <span class="tex-span"><i>m</i></span> lines describe roads in Berland: the <span class="tex-span"><i>j</i></span>-th of them contains two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub> ≠ <i>v</i><sub class="lower-index"><i>j</i></sub></span>), where <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span> are the numbers of cities which are connected by the <span class="tex-span"><i>j</i></span>-th road.</p><p>The cities are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that it is possible to get from any city to any other by following two-ways roads. In Berland there are no roads which connect the same pair of cities. </p>

## Output

<p>In the first line print single integer&nbsp;— the maximum possible value <span class="tex-span"><i>min</i><sub class="lower-index">1 ≤ <i>i</i> ≤ <i>n</i></sub>{<i>r</i><sub class="lower-index"><i>i</i></sub>}</span> after the orientation of roads. </p><p>The next <span class="tex-span"><i>m</i></span> lines must contain the description of roads after the orientation: the <span class="tex-span"><i>j</i></span>-th of them must contain two integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub>, <i>v</i><sub class="lower-index"><i>j</i></sub></span>, it means that the <span class="tex-span"><i>j</i></span>-th road will be directed from the city <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> to the city <span class="tex-span"><i>v</i><sub class="lower-index"><i>j</i></sub></span>. Print roads in the same order as they are given in the input data. </p>





```input1
7 9
4 3
2 6
7 1
4 1
7 3
3 5
7 4
6 5
2 5

```




```output1
4
4 3
6 2
7 1
1 4
3 7
5 3
7 4
5 6
2 5

```


